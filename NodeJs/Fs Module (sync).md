- const { readFileSync, writeFileSync } = reqquire('fs')
- this is another way of using specific methods from a module here we can use its read and write file methods

- Then we use method like  
- const first = readFileSync('./test/first.txt', 'utf8')
- console.log(first)
- takes 2 parameters file path and encoding to use

- Similarly 
- writeFileSync(
'./test/result.txt',
`The Result : ${first}, How are You?`
)

- takes 2 functions one path & second write but also take 3rd parameter called if you add , {flag: 'a' } it will append to file
- writeFileSync(
'./test/result.txt',
`The Result : ${first}, How are You?`,
{ flag: 'a' }
)

