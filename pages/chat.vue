<template>
    <div>
	<Chat 
        :participants="participants"
        :myself="myself"
        :messages="messages"
        :chat-title="chatTitle"
        :placeholder="placeholder"
        :colors="colors"
        :border-style="borderStyle"
        :hide-close-button="hideCloseButton"
        :close-button-icon-size="closeButtonIconSize"
        :submit-icon-size="submitIconSize"
        :submit-image-icon-size="submitImageIconSize"
        :load-more-messages="toLoad.length > 0 ? loadMoreMessages : null"
        :link-options="linkOptions"
        :async-mode="asyncMode"
        :scroll-bottom="scrollBottom"
        :display-header="true"
        :send-images="true"
        :profile-picture-config="profilePictureConfig"
        :timestamp-config="timestampConfig"
        @onImageClicked="onImageClicked"
        @onImageSelected="onImageSelected"
        @onMessageSubmit="onMessageSubmit"
        @onType="onType"
        @onClose="onClose">
        </Chat>
</div>
</template>
<script>
import {Chat} from 'vue-quick-chat';
import 'vue-quick-chat/dist/vue-quick-chat.css';

export default {
    components: {
        Chat
    },
    data() {
        return {
            visible: true,
            participants: [
                {
                    name: 'KARTO.ID',
                    id: 1,
                    profilePicture: 'https://avatars3.githubusercontent.com/u/24291960?s=460&u=9ba0275459158fe59063af2448f8782d3a017b0e&v=4'
                }
            ],
            myself: {
                name: 'Wahid Rizka',
                id: 2,
                profilePicture: 'https://avatars1.githubusercontent.com/u/58039870?s=400&u=5f950d667b4b844b46d8eafa91f402b80565e952&v=4'
            },
            messages: [
                {
                    content: 'Karto adalah.....................',
                    myself: false,
                    participantId: 1,
                    timestamp: {year: 2021, month: 1, day: 4, hour: 20, minute: 10, second: 3, millisecond: 123},
                    type: 'text'
                },
                {
                    content: 'Okay Karto, Terimakasih Karto',
                    myself: true,
                    participantId: 2,
                    timestamp: {year: 2021, month: 1, day: 4, hour: 19, minute: 10, second: 3, millisecond: 123},
                    type: 'text'
                }
            ],
            chatTitle: 'Live Chat KARTO.ID',
            placeholder: 'Ketik Pesan',
            colors: {
                header: {
                    bg: '#f66a0a',
                    text: '#fff'
                },
                message: {
                    myself: {
                        bg: '#f66a0a',
                        text: '#fff'
                    },
                    others: {
                        bg: '#e1e4e8',
                        text: '#444d56'
                    },
                    messagesDisplay: {
                        bg: '#fafbfc'
                    }
                },
                submitIcon: '#f66a0a',
                submitImageIcon: '#f66a0a',
            },
            borderStyle: {
                topLeft: "10px",
                topRight: "10px",
                bottomLeft: "10px",
                bottomRight: "10px",
            },
            hideCloseButton: false,
            submitIconSize: 25,
            closeButtonIconSize: "20px",
            asyncMode: false,
            toLoad: [
                {
                    content: 'Karto Disini',
                    myself: false,
                    participantId: 1,
                    timestamp: {year: 2021, month: 1, day: 4, hour: 10, minute: 10, second: 3, millisecond: 123},
                    uploaded: true,
                    viewed: true,
                    type: 'text'
                },
                {
                    content: "Kenapa sih namanya Karto?",
                    myself: true,
                    participantId: 2,
                    timestamp: {year: 2021, month: 1, day: 4, hour: 19, minute: 10, second: 3, millisecond: 123},
                    uploaded: true,
                    viewed: true,
                    type: 'text'
                },
            ],
            scrollBottom: {
                messageSent: true,
                messageReceived: false
            },
            displayHeader:true,
            profilePictureConfig: {
                others: true,
                myself: true,
                styles: {
                    width: '30px',
                    height: '30px',
                    borderRadius: '50%'
                }
            },
            timestampConfig: {   
                format: 'HH:mm',
                relative: false
            },
            // there are other options, you can check them here
            // https://soapbox.github.io/linkifyjs/docs/options.html
            linkOptions: {
                myself: {
                    className: 'myLinkClass',
                    events: {
                        click: function (e) {
                            alert('Link clicked!');
                        },
                        mouseover: function (e) {
                            alert('Link hovered!');
                        }
                    },
                    format: function (value, type) {
                        if (type === 'url' && value.length > 50) {
                            value = value.slice(0, 50) + '…';
                        }
                        return value;
                    }
                },
                others: {
                    className: 'othersLinkClass',
                    events: {
                        click: function (e) {
                            alert('Link clicked!');
                        },
                        mouseover: function (e) {
                            alert('Link hovered!');
                        }
                    },
                    format: function (value, type) {
                        if (type === 'url' && value.length > 50) {
                            value = value.slice(0, 50) + '…';
                        }
                        return value;
                    }
                }
            }
        }
    },
    methods: {
        onType: function (event) {
            //here you can set any behavior
        },
        loadMoreMessages(resolve) {
            setTimeout(() => {
                resolve(this.toLoad); //We end the loading state and add the messages
                //Make sure the loaded messages are also added to our local messages copy or they will be lost
                this.messages.unshift(...this.toLoad);
                this.toLoad = [];
            }, 1000);
        },
        onMessageSubmit: function (message) {
            /*
            * example simulating an upload callback. 
            * It's important to notice that even when your message wasn't send 
            * yet to the server you have to add the message into the array
            */
            this.messages.push(message);

            /*
            * you can update message state after the server response
            */
            // timeout simulating the request
            setTimeout(() => {
                message.uploaded = true
            }, 2000)
        },
        onClose() {
            this.visible = false;
        },
        onImageSelected(files, message){
            let src = 'https://149364066.v2.pressablecdn.com/wp-content/uploads/2017/03/vue.jpg'
            this.messages.push(message);
            /**
             * This timeout simulates a requisition that uploads the image file to the server.
             * It's up to you implement the request and deal with the response in order to
             * update the message status and the message URL
             */
            setTimeout((res) => {
                message.uploaded = true
                message.src = res.src
            }, 3000, {src});
        },
        onImageClicked(message){
            /**
             * This is the callback function that is going to be executed when some image is clicked.
             * You can add your code here to do whatever you need with the image clicked. A common situation is to display the image clicked in full screen.
             */
            console.log('Image clicked', message.src)
        }
    }
}
</script>