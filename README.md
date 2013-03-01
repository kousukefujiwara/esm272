esm272
======
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html lang='en' xml:lang='en' xmlns='http://www.w3.org/1999/xhtml'>
  <head>
    <meta content='text/html; charset=utf-8' http-equiv='Content-Type' />
    <title>Sankey Javascript Demo: Spread effort 2050 Pathway</title>
    <script src="../ext/raphael.js" type="text/javascript"></script>
    <script src="../ext/jquery.js" type="text/javascript"></script>
    <script src="../js/sankey.js" type="text/javascript"></script>
  </head>
  <body>
    <script type='text/javascript'>
      $(document).ready(function() {
        var sankey = new Sankey();
      
        sankey.stack(0,["Top","Bottom"]);
        sankey.stack(1,["Merge"]);
        sankey.stack(2,["Good","Bad"]);
      
        sankey.setData([["Top",100,"Merge"],["Bottom",50,"Merge"],["Merge",70,"Good"],["Merge",80,"Bad"]]);
        sankey.draw();
    });
      
    </script>
    <h1 style='width:1000px; text-align: center; margin-bottom: 0'>A very simple Sankey Diagram</h1>
    <div style='width:1000px; text-align: center; margin-top: 0'>Move your mouse over the diagram to show values</div>
    <div id='sankey' style="width:1000px;height:1000px">
      &nbsp;
    </div>
  </body>
</html>
