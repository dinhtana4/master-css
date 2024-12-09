display: flex -> set cho thẻ cha. Khi set display: flex, có những thuộc tính liên quan
+ flex-direction: row (mặc định), row-reverse, column, column-reverse
+ align-items: vertically align, stretch (mặc định - giúp các thẻ con bên trong có chiều dài (hoặc chiều ngang if flex-direction: column) bằng nhau - mặt dù content khác nhau), flex-start: canh top hoăc left (ko stretch), flex-end: canh phải hoặc bottom (ko stretch), center: canh giữa, baseline: canh theo dòng chữ đầu tiên
+ flex-wrap: no-wrap (default): ép các thẻ con nằm trên 1 hàng, nếu width tổng thẻ con lớn hơn parent, thì nó sẽ ép width nhỏ lại để đảm bảo các thẻ con nằm trên 1 hàng. wrap: cho phép các thẻ con rớt xuống hàng nếu parent không đủ width
+ justify-content: horizontally align, flex-start: hiển thị ở bên trái, flex-end: hiển thị ở phía bên phải, center: hiển thị trung tâm, space-between: hiển thị 2 bên trái phải - trống ở trung tâm, space-around: khoảng trống sẽ chia đều ở mỗi phần tử, space-evenly: khoảng trống giữa mỗi phần tử bằng nhau
+ flex: 1, khi có 1 khối nằm trong flex có 2 khối con, 1 khối cố định height, khối còn lại sẽ auto theo content, set flex: 1 giúp khối còn lại co - giãn đều với những khối khác trong flex

display: grid
+ grid-column-template: 270px 270px 270px 270px || 50% 50% 50% 50% || 1fr 1fr 1fr 1fr || repeat(4, 1fr) || 200px repeat(2, 1fr) 300px -> chia số lượng columns
+ align-items: stretch, start, end, center (like flex)
+ justify-content: start, end, center, space-between, space-around (like flex).
+ grid-auto-rows: 150px property to set a default size (height) for all rows

Text:
+ white-space: nowrap: hiển thị text trên 1 hàng.
+ overflow: hidden: ẩn/cắt bỏ content khi content dài quá chiều dài thẻ parent
+ text-overflow: ellipsis: hiển thị dấu 3 chấm khi text dài quá chiều dài của thẻ parent
work-break: break-word: cắt xuống hàng theo word.
+ display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical: hiển thị text trên 2 hàng, sau đó mới truncat nếu quá 2 hàng.

Image
+ object-fit: cover: để hình bao phủ full & không bị méo

Margin:
+ margin-top: auto -> đẩy item về bottom
+ margin-bottom: auto -> đẩy item về top
+ margin-left: auto -> đẩy item về right
+ margin-right: auto -> đẩy item về left
+ margin: 0 auto: đẩy item về center

pointer-events: none: loại bỏ event con trỏ trên thẻ