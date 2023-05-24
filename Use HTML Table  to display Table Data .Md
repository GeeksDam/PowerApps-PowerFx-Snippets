/* One of the best practices on Canvas App development is using less controls for app best performance*/

/* To display a collection data or a table inforation that rewuire oly vbiew operation ios best diaplayed using a HTML Text control and format with HTML Table syntax*/

/* I created a small collection to display on my HTML table here*/

Insert HTMLText control to your app 

My Collection Data 

ClearCollect(Data, {Column1:"Data1",Column2:"Data2",Column3:"Data3"},{Column1:"Data11",Column2:"Data22",Column3:"Data33"},{Column1:"Data111",Column2:"Data222",Column3:"Data333"}, {Column1:"Data1111",Column3:"Data3"})


 HTMLText Property : 
 "<center>" & "<b>" & "Data Table" &   "</center>"  & "</b>"&  "<br>" &"<table width='100%' border='1' cellpadding='4' style='border:1px solid black; border-collapse:collapse'>" & "<tr style='background-color:#efefef'>
         <th>Column1 </th> <th> Column2 </th> <th> Column3 </th> 
     </tr> <tr>" &
         Concat(Data,
             "<td>" & Column1 & " </td>
              <td>" & Column2 & " </td>
 <td>" & Column3 & " </td>
    </tr><tr>") & "<tr> <td> Row Count: " &CountRows(Filter(Data,Not(Column1 = Blank()))) & "</td> <td>Row Count: " & CountRows(Filter(Data,Not(Column2 = Blank()))) & "</td> <td> Row Count: " &CountRows(Filter(Data,Not(Column3 = Blank()))) & "</td> </tr>" & 

"</table>" 

![image](https://github.com/GeeksDam/PowerApps/assets/98710158/9629f45c-32c0-49cb-b20e-baebb1c52d09)



