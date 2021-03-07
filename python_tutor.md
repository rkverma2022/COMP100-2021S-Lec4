## LINKS

EXAMPLE: combinations of print and return
Python Tutor link: http://www.pythontutor.com/visualize.html#code=def%20is_even_with_return(%20i%20%29%3A%0A%20%20%20%20%22%22%22%20%0A%20%20%20%20Input%3A%20i,%20a%20positive%20int%0A%20%20%20%20Returns%20True%20if%20i%20is%20even,%20otherwise%20False%0A%20%20%20%20%22%22%22%0A%20%20%20%20print('with%20return'%29%0A%20%20%20%20remainder%20%3D%20i%20%25%202%0A%20%20%20%20return%20remainder%20%3D%3D%200%0A%0Ais_even_with_return(3%29%20%0Aprint(is_even_with_return(3%29%20%29%0A%0Adef%20is_even_without_return(%20i%20%29%3A%0A%20%20%20%20%22%22%22%20%0A%20%20%20%20Input%3A%20i,%20a%20positive%20int%0A%20%20%20%20Does%20not%20return%20anything%0A%20%20%20%20%22%22%22%0A%20%20%20%20print('without%20return'%29%0A%0Ais_even_without_return(3%29%0Aprint(is_even_without_return(3%29%20%29%0A&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false 

---

EXAMPLE: functions as arguments
Python Tutor link: http://www.pythontutor.com/visualize.html#code=def%20func_a(%29%3A%0A%20%20%20%20print('inside%20func_a'%29%0A%0Adef%20func_b(y%29%3A%0A%20%20%20%20print('inside%20func_b'%29%0A%20%20%20%20return%20y%0A%0Adef%20func_c(z%29%3A%0A%20%20%20%20print('inside%20func_c'%29%0A%20%20%20%20return%20z(%29%0A%0Aprint(func_a(%29%29%0Aprint(5%2Bfunc_b(2%29%29%0Aprint(func_c(func_a%29%29%0A&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false

---

EXAMPLE: functions as arguments
Python Tutor link: http://www.pythontutor.com/visualize.html#code=def%20func_a(%29%3A%0A%20%20%20%20print('inside%20func_a'%29%0A%0Adef%20func_b(y%29%3A%0A%20%20%20%20print('inside%20func_b'%29%0A%20%20%20%20return%20y%0A%0Adef%20func_c(z%29%3A%0A%20%20%20%20print('inside%20func_c'%29%0A%20%20%20%20return%20z(%29%0A%0Aprint(func_a(%29%29%0Aprint(5%2Bfunc_b(2%29%29%0Aprint(func_c(func_a%29%29%0A&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false

---

EXAMPLE: returning function objects
Python Tutor link: http://www.pythontutor.com/visualize.html#code=def%20f(%29%3A%0A%20%20%20%20def%20x(a,%20b%29%3A%0A%20%20%20%20%20%20%20%20return%20a%2Bb%0A%20%20%20%20return%20x%0A%20%20%20%20%0Aval%20%3D%20f(%29(3,4%29%0Aprint(val%29%0A&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false

---

EXAMPLE: hader scope example from slides
Python Tutor link: http://www.pythontutor.com/visualize.html#code=def%20g(x%29%3A%0A%20%20%20%20def%20h(%29%3A%0A%20%20%20%20%20%20%20%20x%20%3D%20'abc'%0A%20%20%20%20x%20%3D%20x%20%2B%201%0A%20%20%20%20print('in%20g(x%29%3A%20x%20%3D',%20x%29%0A%20%20%20%20h(%29%0A%20%20%20%20return%20x%0A%0Ax%20%3D%203%0Az%20%3D%20g(x%29&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false

---

EXAMPLE: complicated scope, test yourself!
Python Tutor link: http://www.pythontutor.com/visualize.html#code=def%20f(x%29%3A%0A%20%20%20x%20%3D%20x%20%2B%201%0A%20%20%20print('in%20f(x%29%3A%20x%20%3D',%20x%29%0A%20%20%20return%20x%0A%0Ax%20%3D%203%0Az%20%3D%20f(x%29%0Aprint('in%20main%20program%20scope%3A%20z%20%3D',%20z%29%0Aprint('in%20main%20program%20scope%3A%20x%20%3D',%20x%29%0A%0Adef%20g(x%29%3A%0A%20%20%20%20def%20h(x%29%3A%0A%20%20%20%20%20%20%20%20x%20%3D%20x%2B1%0A%20%20%20%20%20%20%20%20print(%22in%20h(x%29%3A%20x%20%3D%20%22,%20x%29%0A%20%20%20%20x%20%3D%20x%20%2B%201%0A%20%20%20%20print('in%20g(x%29%3A%20x%20%3D%20',%20x%29%0A%20%20%20%20h(x%29%0A%20%20%20%20return%20x%0A%0Ax%20%3D%203%0Az%20%3D%20g(x%29%0Aprint('in%20main%20program%20scope%3A%20x%20%3D%20',%20x%29%0Aprint('in%20main%20program%20scope%3A%20z%20%3D%20',%20z%29%0A&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false

