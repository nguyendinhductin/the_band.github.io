1. HTML - HyperText Markup Language

Giúp người dùng tạo và cấu trúc các thành phần trong trang web hoặc ứng dụng, phân chia các đoạn văn, heading, links,...

2. CSS - Cascading Style Sheet language

Dùng để tạo phong cách và định kiểu cho những yếu tố được viết dưới dạng ngôn ngữ đánh dấu, như là HTML

3. thẻ meta charset = "utf-8"

để hỗ trợ web tiếng việt

4. a - anchor

5. Atribute - thuộc tính của thẻ HTML

title, class, id, style, onclick...

6. 3 cách viết CSS trong HTML

- Internal: dùng cặp thẻ link Style
- External: thư mục
- Inline: style

7. CSS Selector

Trong CSS, CSS selectors là các cách chúng ta sử dụng để chọn ra các phần tử (elements) mà chúng ta muốn "style" cho chúng. Có 2 CSS selectors thân thuộc với chúng ta nhất là id và class.

8. Priority - sự ưu tiên

- Internal, External: cái nào trc thì được ưu tiên
- Inline: 1000
- Id: 100
- Class: 10
- tags: 1
- !important >1000

9. CSS Variable

sử dụng dấu "--": --text-color
để xét toàn file HTML (global)
:root {}

10. font-size mặc định của web là 16px

- rem phụ thuộc vào thẻ html{
  font-size: 20px => 1rem = 20px
  }
- em phụ thuộc vào thẻ gần nhất của nó
- vh, vw: viewport height, width: theo màn hình trình duyệt
- % tính phụ thuộc vào thẻ bao bọc nó

11. Thêm rel="noopener" khi sử dụng target="\_blank"

12. html -> font-size: 62.5% = 10px -> 1.6rem = 16px

13. CSS pseudo-classes : Lớp giả css
    :root
    :hover
    :active -> click
    :first-child
    :last-child

14. CSS pseudo-elements : Phần tử giả
    ::before
    ::after
    ::first-letter
    ::first-line
    ::selection: bôi đen thay đổi

15. Mặc định thẻ div là display:block

16. Sử dụng box-sizing:border-box cho box để kích thước của box không thay đổi

17. Short hand background-image(url), no repeat, position / contain

18. CSS position

- Relative: tương đối, nếu set vị trí cho nó sẽ có thể đè lên các phần tử khác.
- Absolute: tuyệt đối, sử dụng trong đối tượng con, nó sẽ tìm đối tượng cha có thuộc tính position gần nhất để áp dụng trên nó
- Fixed: để cố định khối khi scroll trang
- Sticky: bám dính kèm với thuộc tính position: -webkit-sticky

19. Căn giữa thuộc tính trong khối
    text-align: center -> chiều ngang
    line-height: = với khối box -> chiều dọc

---

display: flex | cho thuộc tính con margin: auto -> căn giữa tương tự

---

align-items: center -> chiều cao
justify-content: center -> chiều dọc

- Với position
  .box{
  height: 100px;
  position: relative;
  }

  h3(thecon){
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  }

20. Flexbox

Codepen.io
(Flexbox Playground)

21. BEM (Block Element Modifier)

## Định nghĩa

- Là tiêu chuẩn đặt tên Class khi viết CSS

## Ý nghĩa

- Block: Khối
- Element: Thành phần trong khối
- Modifier: Bổ sung ý nghĩa cho `Block` hoặc `Element`

## Sử dụng để?

- Mỗi người đặt một kiểu
- Members đặt class trùng nhau, CSS đè lên nhau

## Cú pháp

<!-- - .block -->
<!-- - .block__element -->

<!-- - .block--modifier -->
<!-- - .block__element--modifier -->

## Ví dụ

<div class="card card--success">
  <h3 class="card__heading">Saved!</h3>
  <p class="card__desc">hihi</p>
  <div class="card__btn">Oke</div>
</div>

<div class="card card--error">
  <h3 class="card__heading">Saved!</h3>
  <p class="card__desc">hihi</p>
  <div class="card__btn">Oke</div>
</div>

## Tính ứng dụng

- Xây dựng layout Web
- Xây dựng thành phần trên Web
