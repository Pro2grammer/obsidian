const { readFile, writeFile } = require('fs')
readFile('./test/first.txt','utf8',(err,result) => {
if (err) {
console.log(err)
return
}
console.log(result)
})

here we use readfile only it is async and also we use a function which has 2 pre-defined paramenters 1st error and 2nd result .

Also we use encoding type eg. 'utf8' in between path and function other wise it gives buffer.


- now if we use more read or writes we do it inside first, ie 2nd inside 1st , 3rd inside 2nd (we do it for access to variables)
- ie

readFile('./test/first.txt','utf8',(err,result) => {
if (err) {
console.log(err)
return
}
const first = result; 
readFile('./test/text.txt','utf8',(err,result2) => {
if (err) {
console.log(err)
return
}
const second = result2
writeFile(
'./test/result_new.txt',
`The result String : ${first}, ${second}`,
(err, result) =>{
if (err) {
console.log(err)
return
}
console.log(result)
}
)
})
})

- also ere we write file like shown above we have to use function with err and result also
