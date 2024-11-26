display: flex -> set cho thẻ cha. Khi set display: flex, có những thuộc tính liên quan
+ flex-direction: row (mặc định), row-reverse, column, column-reverse
+ align-items: stretch (mặc định - giúp các thẻ con bên trong có chiều dài (hoặc chiều ngang if flex-direction: column) bằng nhau - mặt dù content khác nhau), flex-start: đưa thẻ nổi lên top (hoặc left), flex-end: đưa thẻ nổi xuống bottom (hoặc right), center: canh giữa, baseline: canh theo dòng chữ đầu tiên
+ flex-wrap: no-wrap (default): ép các thẻ con nằm trên 1 hàng, nếu width tổng thẻ con lớn hơn parent, thì nó sẽ ép width nhỏ lại để đảm bảo các thẻ con nằm trên 1 hàng. wrap: cho phép các thẻ con rớt xuống hàng nếu parent không đủ width
+ justify-content: flex-start: hiển thị ở bên trái, flex-end: hiển thị ở phía bên phải, center: hiển thị trung tâm, space-between: hiển thị 2 bên trái phải - trống ở trung tâm, space-around: khoảng trống sẽ chia đều ở mỗi phần tử, space-evenly: khoảng trống giữa mỗi phần tử bằng nhau

display: grid
+ grid-column-template: 270px 270px 270px 270px || 50% 50% 50% 50% || 1fr 1fr 1fr 1fr || repeat(4, 1fr) -> chia số lượng columns
+ align-items: stretch, start, end, center (like flex)
+ justify-content: start, end, center, space-between, space-around (like flex)

Text:
+ white-space: nowrap: hiển thị text trên 1 hàng.
+ overflow: hidden: ẩn/cắt bỏ content khi content dài quá chiều dài thẻ parent
+ text-overflow: ellipsis: hiển thị dấu 3 chấm khi text dài quá chiều dài của thẻ parent
work-break: break-word: cắt xuống hàng theo word.
+ display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical: hiển thị text trên 2 hàng, sau đó mới truncat nếu quá 2 hàng.

Image
+ object-fit: cover: để hình bao phủ full & không bị méo