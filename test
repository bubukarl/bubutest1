func add( n1:String, n2 :String) ->String{
    var n1 = n1
    /*if n2.characters.count > n1.characters.count {
        n1 = "" + n1
        print(n1)
    }
 */
    let a1:[Int] = Array(n1.characters).reversed().map() { Int(String($0))!}
    let a2:[Int] = Array(n2.characters).reversed().map() { Int(String($0))!}
    var result=[Int](repeating : 0, count: a2.count + 1)
    
    var carry:Int = 0
    for var i in 0...a2.count-1{
        if i < a1.count {
        result[i] = a1[i] + a2[i] + carry
        carry = result[i]/10
            result[i] = result[i] % 10
        }else {
            result[i] = a2[i] + carry
            carry = 0
        }
        i = i + 1
    }
    result[a2.count] = carry
    

    var Tresult = result.reversed().map{String($0)}
	//print(Tresult[0])
	if Tresult[0] == "0" {
	Tresult[0] = ""
	}
	//print (Tresult.count-1, Tresult[0], Tresult[1])

    return Tresult.joined(separator:"")
}
func f(n:String) ->String{
    if n == "0" {
        return "0"
    }else if n == "1"{
        return "1"
    }else if n == "2"{
        return "1"
}else {
        var f0:String = "0", f1:String = "1", f2:String = "1"
        let x = Int(n)!
    for  var index in 3...x{
        f0 = f1
        f1 = f2
        f2 = add(n1: f0, n2: f1)
        index = index + 1
    }
    return f2

    }
}
print(f(n: "5278"))









