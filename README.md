<h1 align="center">

<p align="center">
  <img src="https://i.imgur.com/czovy76.png" height="300" width="600" />
</p>

<p align="center">
    <img src="https://img.shields.io/badge/vue-js-green">
    <img src="https://img.shields.io/badge/no%20dependencies-vanillajs-green">
    <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-green.svg" />
    <img src="https://img.shields.io/badge/license-MIT-green" />
</p>


    Simple vue component (No dependencies)

If this project has helped you out, please support me with a star 🌟

</h1>

# vue-simple-card

A simple card component made with VueJS, with a icon (image), title and content, it's totally customizable

## Props

```
- bcolor: background color
- headerLink: a link on the header div (the link is attached to the image and the title)
- titleFontFamily: title's font family
- titleFontSize: title's font size
- titleFontColor: title's font color (css color property)
- icon: icon (the url to the image)
- title: Title Text
- content: the text to show
- contentColor: content text font color
- contentFontFamily: content's font family
- size: height of the card
- width: width of the card
```

## Usage

```js

<VueSimpleCard 
                        title="Vue simple card" 
                        title-font-size="1.3rem" 
                        title-font-family="'Open Sans',sans-serif"
                        title-font-color="white"
                        header-link="https://diegofelipe.io" 
                        icon="https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png" 
                        width="19rem"
                        content="Mussum Ipsum, cacilds vidis litro abertis. A ordem dos tratores não altera o pão duris. Viva Forevis aptent taciti sociosqu ad litora torquent. Tá deprimidis, eu conheço uma cachacis que pode alegrar sua vidis. Atirei o pau no gatis, per gatis num morreus.

                        Praesent malesuada urna nisi, quis volutpat erat hendrerit non. Nam vulputate dapibus. Sapien in monti palavris qui num significa nadis i pareci latim. Vehicula non. Ut sed ex eros. Vivamus sit amet nibh non tellus tristique interdum. Nullam volutpat risus nec leo commodo, ut interdum diam laoreet. Sed non consequat odio.

                        Nec orci ornare consequat. Praesent lacinia ultrices consectetur. Sed non ipsum felis. Casamentiss faiz malandris se pirulitá. Si u mundo tá muito paradis? Toma um mé que o mundo vai girarzis! Copo furadis é disculpa de bebadis, arcu quam euismod magna.

                        Em pé sem cair, deitado sem dormir, sentado sem cochilar e fazendo pose. Quem manda na minha terra sou euzis! Cevadis im ampola pa arma uma pindureta. Detraxit consequat et quo num tendi nada." 
                        content-color="white"
                        content-font-family="'Open Sans',sans-serif"
                        bcolor="linear-gradient(to right, #11998e, #38ef7d)"
                        size="8rem"
                    >
                   
                    
                        
                    </VueSimpleCard>
```
