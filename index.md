<script type="text/javascript">
    function getDay(date1, date2) {
      var ms = Math.abs(date2 - date1);
      // 两个日期相减得到毫秒数  1s=1000ms
      var s = ms / 1000; // 毫秒转为秒
      var day = Math.floor(s / 3600 / 24); //天
      var hour = Math.floor(s / 3600 % 24); //小时
      var minute = Math.floor(s % 60);  //分
      return "相差" + day + "天" + hour + "小时" + minute + "分";
    }
    var oDate1 = new Date(); // 获取当前日期
    var oDate2 = new Date("2022-6-14 8:00:00"); // 指定未来时间
    document.write(getDay(oDate1, oDate2));
  </script>
