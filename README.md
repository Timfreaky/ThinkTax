# ThinkTax
Source code for ThinkTax (Wordpress)

In the following folder, you will find everything you need to continue ThinkTax in its actual state.

You will find every plugin I needed to develop the website:

- Ultimate Member
- CSS & Javascript Toolbox
- Contact Form 7

Some code has been added for every scenario:
-------------------------------------------------------------------------------------------------------------
Custome Table:
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
    <body>
    <table>
    <tr>
    <th>Recommandations</th>
    <th>Renvois de bases</th>
    <th>Sources</th>
    </tr>
        <tr>
            <td></td>
            <td>[1]Art. 113 al. 4 LIFD </br>
                [2]Art. 214 al. 1 LIFD </br>
                [3]Art. 214 al. 2 LIFD </br>
                [4]Art. 11 LHID </br>
                [5]Art. 11 LIPP V </br>
                [6]Art. 12 al. 3 LIPP V </br>
                [7]Art. 129 CC </br>
                [8]Art. 134 CC
            </td>
            <td>- Droit fiscal suisse, Recueil de cas pratique - Jean-Frédéric Maraia, Cas Pratiques, 2008 </br>
                </br>
                www.easydivorce.ch: Catégorie : Procédure de divorce </br>
                </br>
                www.divorce.ch: Modification du jugement de divorce
            </td>
        </tr>
    </table>
    </body>
</html>

--------------------------------------------------------------------------------------------------------------------
Custome Life Line:

<script type="text/javascript" src="https://www.google.com/jsapi?autoload={'modules':[{'name':'visualization',
       'version':'1','packages':['timeline']}]}"></script>
<script type="text/javascript">

google.setOnLoadCallback(drawChart);
function drawChart() {
  var container = document.getElementById('example2.1');
  var chart = new google.visualization.Timeline(container);
  var dataTable = new google.visualization.DataTable();

  dataTable.addColumn({ type: 'string', id: 'Term' });
  dataTable.addColumn({ type: 'string', id: 'Name' });
  dataTable.addColumn({ type: 'date', id: 'Start' });
  dataTable.addColumn({ type: 'date', id: 'End' });

  dataTable.addRows([
    [ 'Evénement', 'Divorce: pension alimentaire', new Date(2006, 1, 1), new Date(2010, 1, 1) ],
    [ 'Evénement', 'Frais avocat', new Date(2010, 1, 1),  new Date(2014, 1, 1) ],
    [ 'Evénement', 'Incapacité de travail', new Date(2010, 1, 1),  new Date(2012, 6, 1) ],
    [ 'Evénement', 'Divorce: remariage', new Date(2013, 1, 1), new Date(2015, 5, 1) ]]);
    
    var options = {
    timeline: {groupByRowLabel: false}
    };

  chart.draw(dataTable, options);
}
</script>

<div id="example2.1" style="height: 200px;"></div>
-------------------------------------------------------------------------------------------------------------------
You will find everything else you need for developing the site in its folder.


