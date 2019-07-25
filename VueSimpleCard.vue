<template>
    <div class="main-card-container" :style="styleObject">
        <div class="mcard-content">
            <div class="mcard-header">
                <a :href="headerLinkData.src" class="mcard-header-link">
                    <img :src="iconData.src" class="mcard-header-icon">
                    <div class="mcard-header-title" :style="[...fontTitleData]">
                        <div class="mcard-header-title-content">{{ title }}</div>   
                    </div>
                </a>
            </div>
            <div class="mcard-body">
                <span class="mcard-body-content" :style="[...contentData]">{{ content }}</span>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            bcolor: {
                type: String,
                required: false,
                default: "linear-gradient(to right, #11998e, #38ef7d)"
            },
            headerLink: {
                type: String,
                required: false,
                default: "#"
            },
            titleFontFamily: {
                type: String,
                required: false,
            },
            titleFontSize: {
                type: String,
                required: false,
                default: "1.3em"
            },
            titleFontColor: {
                type: String,
                required: false,
                default: "white"
            },
            icon: {
                type: String,
                required: true
            },
            title: {
                type: String,
                required: true,
                default: "Title"
            },
            content: {
                type: String,
                required: true,
                default: "Mussum Ipsum, cacilds vidis litro abertis. Atirei o pau no gatis, per gatis num morreus. Suco de cevadiss, é um leite divinis"
            },
            contentColor: {
                type: String,
                required: false,
                default: "white"
            },
            contentFontFamily: {
                type: String,
                required: false
            },
            size: {
                type: String,
                required: false,
                default: "10rem"
            },
            width: {
                type: String,
                required: false,
                default: "18rem"
            }
        },        
        data() {
            return {
                styleObject: {
                    background: this.bcolor,
                    '--mcard-height': this.size,
                    width: this.width
                },
                fontTitleData: {
                    fontFamily: this.titleFontFamily,
                    fontSize: this.titleFontSize,
                    color: this.titleFontColor
                },
                contentData: {
                    color: this.contentColor,
                    fontFamily: this.contentFontFamily
                },
                headerLinkData: {
                    src: this.headerLink
                },
                iconData: {
                    src: this.icon
                }
            }
        },
    }
</script>

<style scoped>
    .main-card-container {
        height: calc(var(--mcard-height));
    }
    .mcard-content {
        padding-bottom: calc(var(--mcard-height) * 0.05);
    }
    .mcard-header {
        height: calc(var(--mcard-height) * 0.4);
        padding-top: calc(var(--mcard-height) * 0.05);
        margin-left: .8rem;
    }
    .mcard-header-link {
        display: flex;
        flex-direction: row;
        justify-content: flex-start; /* For main axis */
        align-items: flex-start; /* for cross axis */ 
        text-decoration: none;
        color: inherit;
    }
    .mcard-header-icon {
        height: calc(var(--mcard-height) * 0.3);
    }
    .mcard-header-title {
        height: calc(var(--mcard-height) * 0.3);
        overflow: hidden;
    }
    .mcard-header-title-content {
        height: calc(var(--mcard-height) * 0.2);
        margin-left: .7rem;
        overflow: hidden;
    }
    .mcard-body {
        display: flex;
        justify-content: flex-start;
        margin-left: .8rem;
        margin-right: .8rem;
        text-align: justify;
    }
    .mcard-body-content {
        height: calc(var(--mcard-height) * 0.5);
        overflow: hidden;
    }
</style>

