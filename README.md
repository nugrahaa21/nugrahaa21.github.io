    <!-- JAVASCRIPT AT THE BOTTOM TO REDUCE THE LOADING TIME  -->
    <!-- CORE JQUERY SCRIPTS --> <script src="js/jquery.js"></script>
<script src="js/jQuery-2.2.0.min.js"></script>

    <!-- Bootstrap Core JavaScript -->
    <script src="js/bootstrap.min.js"></script>

    <script src="js/jquery-1.11.2.min.js"></script>
        <script src="bootstrap/js/bootstrap.js"></script>
        <script src="datatables/jquery.dataTables.js"></script>
        <script src="datatables/dataTables.bootstrap.js"></script>
    
    <script>
  $(function () {
    $("#lookup").DataTable();
 $("#example1").DataTable();
    $('#example2').DataTable({
      "paging": true,
      "lengthChange": false,
      "searching": false,
      "ordering": true,
      "info": true,
      "autoWidth": false
    });
  });
</script>



<!-- Print Preview JS --> 
    <script>
      function openPDF() {
    var yourDOCTYPE = "<!DOCTYPE html>"; // your doctype declaration
    var printPreview = window.open('about:blank', 'print_preview', "resizable=yes,scrollbars=yes,status=yes");
    var printDocument = printPreview.document;
    printDocument.open();
    printDocument.write(yourDOCTYPE+
               "<html>"+
                   document.getElementById("pdf").innerHTML+
               "</html>");
    printDocument.close();

    }
    window.openPP = openPP;
    </script>
<script>
  function cetakData(){
    document.getElementById("tanggalCetak").innerHTML = document.getElementById("myDate").value;
    document.getElementById("namaCetak").innerHTML = document.getElementById("nama").value;    
    document.getElementById("alamatCetak").innerHTML = document.getElementById("alamat").value;
}
</script>


  <script type="text/javascript">
  function SetDate()
  {
  var date = new Date();
  var day = date.getDate();
  var month = date.getMonth() + 1;
  var year = date.getFullYear();

  if (month < 10) month = "0" + month;
  if (day < 10) day = "0" + day;

  var today = day + "-" + month + "-" + year;


  document.getElementById('myDate').value = today;
  }
  </script>
</body>
</html>
