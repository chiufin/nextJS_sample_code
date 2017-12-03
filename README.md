# Next.js SampleCode

[next.js tutorial](https://learnnextjs.com/)

```
npm install --save next react react-dom
npm run dev
```

## Fetures
### [Link](https://github.com/zeit/next.js#routing)
1. import next/link - client side router
    - record in location/history 
2. style only apply on <a>, <button>
    - Link only handle router matters

### Pages directory is meaningful
1. like file system
2. other directories like components can change their name

### Route Masking
1. as -> this can use "backword" / "forward" btns, but cannot work when entering "refresh" btn
```
<PostLink id="hello-nextjs" title="Hello Next.js"/>

<Link as={`/p/${props.id}`} href={`/post?title=${props.title}`}>
    <a>{props.title}</a>
</Link>
```
### [Express Server](https://github.com/zeit/next.js#custom-server-and-routing)

### Data fetching in client or server side
```
getInitialProps
```
1. first router will be triggered by server side
(enter in localhost:3000 / localhost:3000/p/33618)
2. enter link to other pages will be triggered by client side
