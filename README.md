<?php
    for($counter = 1; $counter <= 6; $counter++)        
    {
        print("<B>counter is $counter</B><BR>\n");  
?>
<?php
    
    print("<i><B>距离星期一还有几天？</B></i>\n");
    print("<OL>\n");
    for($currentDate = date("U");          
        date("l", $currentDate) != "Monday";    
        $currentDate += (60 * 60 * 24))     
    {
        print("<LI>" . date("l", $currentDate) . "\n");
    }

  
