# Overview

## Introduction

Coral Spectrum has roots as an internal Open Development project, with core volunteers working on this problem since 2012. 
As of 2016, the effort has become part of the One Adobe & Cloud Platform effort, which means building a full Coral Spectrum 
team that includes Exec Leadership, PgM, PM, EM, Dev, and QE members. Coral Spectrum is also becoming a One Adobe Technical 
Standard, meaning it will be used as the default platform for web projects.

## Unified Experience

Our vision is to create consistent Adobe experiences by providing a complete, easy to use library of HTML components. 
Standardization on Coral Spectrum allows teams to reduce code duplication and variation and encourages company wide collaboration. 
This reduction in effort means teams can focus on meeting customer needs, not reinventing the wheel. Use of Coral Spectrum also 
enables easy, unified design updates, and provides a library that is under Adobe’s full control.

## Enhanced API

Coral Spectrum's components are essentially extended DOM elements. We enhance the existing API with additional functionality, 
as well as providing some patterns that aren't available with native HTML alone. Since we expose a JavaScript API that’s 
based on the native DOM API and has all of the same methods as any other HTML element instance, anyone familiar with the 
DOM already knows most of the API works. 

Most API is available via markup, so don’t have to write JavaScript for most basic uses. All you have to do is write 
the markup for a component, just like you would a normal HTML element.

## Future Thinking

Coral Spectrum is pushing the web forward by leveraging the [Web Components](https://www.webcomponents.org/introduction) specification. 
However, given the landscape of browser implementation and the state of the polyfill ecosystem, we decided to only implement 
[Custom Elements v1](https://html.spec.whatwg.org/multipage/custom-elements.html) at this time.

A strong advantage Coral Spectrum derives from custom elements is the ability to hide many implementation details from the consumer. 
More to the point, we found that designs become closely tied to their markup. The use of custom elements allows much more 
freedom to change the underlying markup that supports those elements. This makes the exposed API smaller and more explicit, 
resulting in a lower risk of updates to Coral Spectrum needing to introduce breaking changes.

In addition, every Coral component is an HTML element. This give us the ability to create components from markup or JavaScript 
and lets us treat them like any other native element, setting properties, appending them in the DOM, etc. 

## Spectrum

The current default theme is is an implementation of the [Spectrum](https://spectrum.adobe.com) design specifications, Adobe’s design system.
Spectrum provides elements and tools to help product teams work more efficiently, and to make Adobe’s applications more cohesive.

Coral Spectrum leverages the [Spectrum CSS](https://github.com/adobe/spectrum-css) framework to style 
components including the [Spectrum SVG icons](https://spectrum.adobe.com/page/icons).   

## Built-in Accessibility and Keyboard support 

Having an inaccessible application can mean thousands of dollars of fines if you land a government contract. 
It also means alienating an entire segment of society by making your application completely unusable to them. 
To help you avoid this, we’ve made it a rule that every Coral Spectrum component should be accessible. We’ve also built a few 
things into Coral Spectrum to make implementing accessibility easier for component authors and consumers alike.
 
## Internationalization support
 
Coral Spectrum provides a robust internal system for internationalization of its strings. 
This is done via an internal Adobe process.
 
Supported languages are :

Language family | Language tag | Language variant
--- | --- | ---
English | en-US | American English
French | fr-FR | Standard French
German | de-DE | Standard German
Italian | it-IT | Standard Italian
Spanish | es-ES | Castilian Spanish
Portuguese | pt-BR | Brazilian Portuguese
Japanese | ja-JP | Standard Japanese
Korean | ko-KR | Standard Korean
Chinese | zh-CN | Mainland China, simplified characters
Chinese | zh-TW | Taiwan, traditional characters
Dutch | nl-NL | Netherlands Dutch
Danish | da-DK | Standard Danish
Finnish | fi-FI | Standard Finnish
Norwegian | no-NO | Standard Norwegian
Swedish | sv-SE | Standard Swedish
Czech | cs-CZ | Standard Czech
Polish | pl-PL | Standard Polish
Russian | ru-RU | Standard Russian
Turkish | tr-TR | Standard Turkish

## Browser Support

Coral Spectrum is designed to support the following browsers:
* Chrome (latest)
* Safari (latest)
* Firefox (latest)
* Edge (latest)
* IE 11
* iOS 7+
* Android 4.4+

## Backwards Compatibility

Coral Spectrum ships by default a compatibility package to support the CoralUI 3.x way to register elements `Coral.register`. 
Custom Coral components using Custom Elements v0 are therefore still supported although we highly encourage to migrate 
to Custom Elements v1 as it'll become the Web standard. 



