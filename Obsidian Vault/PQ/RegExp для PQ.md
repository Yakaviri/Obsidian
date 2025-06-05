let fx=(txt as text, regex as text, delim as text)=> 
    Web.Page( "var x = '" & txt & "'; 
        var delim = '" & delim & "'; 
        var pattern = /" & regex & "/gi; 
        var result = x.match(pattern).join(delim); 
        document.write(result);") in 
    fx