
const isName = true

inside {isName ? name : "someone"}
here it checks if isname condition rue then runs name on true and someone on false



like div in html we use react fragment in react
like:
<>here goes the data</>

{name ? (<>

Here 
</>
):(

<h1>test2</h1>
<h2>test3</h2>

)}

here we dont use react fragment like in test 2  and 3 it will give error it doesnt allow more than 1 element without fragment, so wrap it in react fragment <> </>