




function main(){ 
                          
     var n = parseInt(document.getElementById("no of nodes").value);
     console.log(n);
     
     var a = document.getElementById("adj").value.split("\n");
     var v = document.getElementById("values").value.split(' ');  
     
             
     var stack =[] ; 
     var status = [] ; 
     var mat = [] ;
     var count = 0 ;
     var dfs = [];
      
     for(var i = 0 ; i < n ; i++) 
     {
          mat[i] = [];
          status[i]=0;
          dfs[i] = 0;
          for(var j = 0 ; j< n ; j++) 
          { 
               mat[i][j] = parseInt(a[i][j]) ;
               
           }
      } 
      console.log(mat);
      
      
      stack.push(0); 
      status[0]= 1 ; 
      console.log(status);
      
      while(count!=n)
      {
          var node = stack.pop();
          dfs[count] = node;
          count++ ;
          
          for(var i = 0 ; i< n ;i++) 
          {
               
              if(mat[node][i] !=0 && status[i] == 0)
              {
              stack.push(i) ;
              status[i]=1 ;
              }
           }
       }
       var s="";
       for(var i = 0 ;i < n ;i++)
       s = s + v[dfs[i]] + "->";
       
       s=s + "End" ;
       console.log(s);
       document.getElementById("output1").style.display="block";
      
       document.getElementById("output2").innerHTML =  s  ;
       
       
       
       
       
}
             







