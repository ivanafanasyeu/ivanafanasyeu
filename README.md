# Hi, I'm Ivan Afanasyeu
Here is my github profile. I almost don't use github, cause working with close or private companies.
I'm gonna use this page as an informative resource for myself to save helpful links & gists.
For know me better, here is my [LinkedIn](https://www.linkedin.com/in/ivanafanasyev/)

## Tutorials
| Tutorials | Description | Link |
| --- | --- | --- |
| developerway | A bunch of tutorial, mostly about the react | https://www.developerway.com/ |


## Deploy
- Azure
- AWS
- Vercel

## Practice Code
| Tutorials | Description | Link |
| --- | --- | --- |
| Coderbyte | Practice Code solutions | https://coderbyte.com/ |

## Tools
| Tool | Description | Link |
| --- | --- | --- |
| Tabnine | AI assistant. Remain privacy | https://www.tabnine.com/ |
| Garden | ??? | https://garden.io/ |
| Free SSL certificate | ??? | https://github.com/FiloSottile/mkcert |
| EasyMoney | Lib for TS and JS for money | https://github.com/frolovdev/easymoney |


## Mail Services
| Mail | Description | Link |
| --- | --- | --- |
| EmailJS | easy to use. cheap | https://www.emailjs.com/ |
| Mailerlite | Marketing emails. ???? | https://www.mailerlite.com/ |
| TransactionalEmail | Transactional Email?? | https://sendamply.com/ |
| WYSWYG | The headless editor | https://tiptap.dev/ |
| Markdown | - | https://www.npmjs.com/package/marked | 
| React Multi Carousel | - | https://www.npmjs.com/package/react-multi-carousel |
| React Mask | - | https://github.com/pedrosoares/react-the-mask |

## CMS's
| CMS | Description | Link |
| --- | --- | --- |
| Sanity | - . p.s. partner with Next.js | https://www.sanity.io/ |
| Contentful | - | https://www.contentful.com/ |



# Best Practices
## Theming
Use cookie + CSS
In result we get media + override using styled variables and controlled theme provider.
https://github.com/juliaqiuxy/theming-demo

## Fonts loading
1. Use woff2 Use woff before old formats. IE11 - use woff1, IE - use other formats  p.s. Convert ttf to woff2, using onlineconverter 
2. Use font-display font-display: swap; font-display: block; если предпочитаем, чтобы браузер скрывал текст, пока шрифт не загрузится font-display: fallback; если не загружается за 3с, то будет использовать fallback шрифт font-display: optional; если не загружается шрифт за 100ms, то будет использоваться fallback шрифт 
3. Use preload <link rel=“preload” href=“…” as=“font” type=“font/woff2” crossorigin />  p.s. preload только для одного формата от каждого шрифта woff. 
4. Use self-hosted fonts

## Images
1. Use attributes: alt, width, height, srcset or sizes
2. limit pixel density to 2x (3x, 4x weight much more but do not do enough effect for it)
3. add <source> to <picture> with image formats. Try to use WebP\AVI
4. request image early if we really need it (like header bg image, or smth on top)
```html
<link rel="preload" as="image" href="image url" imagesrcset="" imagesizes="" />
```
5. Placeholder trick:
```html
<img
loading="lazy"
decoding="async"
/>
// background-size: cover;
// background-image: url()data:image/svg+xml;base64;[svg text];"
```

## CSS better rendering
content-visibility: auto; //more for Chrome   

## Mobile inputs
https://better-mobile-inputs.netlify.app/
