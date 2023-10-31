
const http = require('http')
const server = http.createServer((req,res)=>{
res.write('Welcome ot my Webpage')
res.end()
})
server.listen(5000)

simple sever.

now with logic you can use request to perform action eg req.url
const http = require('http')
const server = http.createServer((req,res)=>{
if(req.url === '/'){
res.end('Welcome ot my Webpage')
}
if(req.url === '/about'){
res.end('Here is our about page')
}
res.end(`
<h1> oops!</h1>
<p>We can't seen to find the page you are looking for</p>
<a href="/"> Back Home</a>
`)
})
server.listen(4000)