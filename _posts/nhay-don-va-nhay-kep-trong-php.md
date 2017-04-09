Nháy đơn và nháy kép ?

Thỉnh thoảng, trong khi code PHP chắc hẳn chúng ta đã từng nhìn thấy dấu nháy đơn và nháy kép xuất hiện trong các đọan code. Và ngay cả bản thân chúng ta cũng đã từng sử dụng qua lại giữa dấu nháy đơn hoặc nháy kép như một thói quen mà không hề hiểu rõ được khi nào nên dùng nháy đơn hoặc nháy kép. Bài viết này có thể sẽ giúp bạn phân biệt được khi nào nên dùng nháy đơn hoặc nháy kép

 

Dấu nháy đơn

Dấu ngoặc đơn không thể Parse được giá trị của biến.

Có nghĩa là, những gì được viết trong dấu nháy đơn sẽ được hiển thị ra y hệt mà không được Parse. Các kí hiệu như \n hoặc \t sẽ không được xác định

Ví dụ:

{% highlight php %}
  // khai báo biến + giá trị
  $bien = "gia tri";
  echo 'In du lieu $bien';
{% endhighlight %}
