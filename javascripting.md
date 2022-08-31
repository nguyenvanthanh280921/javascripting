# Introduction

**JavaScript** là một ngôn ngữ lập trình biên dịch, sử dụng trên đa nền tảng và được thông dịch, còn được gọi là ngôn ngữ kịch bản cho các trang web. Javascript được dùng trong trang web bên cạnh HTML và CSS. JavaScript có thể được sử dụng cho các phát triển phía Client cũng như các phát triển phía Server. Javascript vừa là loại ngôn ngữ mệnh lệnh vừa là ngôn ngữ khai báo. JavaScript chứa một thư viện tiêu chuẩn của các đối tượng, như Mảng , Ngày tháng và Toán học , và một tập hợp cốt lõi của các phần tử ngôn ngữ như toán tử , cấu trúc điều khiển và câu lệnh . 

# Valiable

- **Valiable** là các vùng chứa được đặt tên để lưu trữ các giá trị dữ liêu.
- Valiable được khai báo bằng các từ khóa **var**, **let**, **const**

# String

- Là một chuỗi các ký tự như chữ cái, số, dấu câu, dấu cách,...
- Chuỗi thường được viết trong dấu ngoặc đơn hoặc dấu ngoặc kép ('...',"...").
> *'this is a string'* hoặc *"this is a string"*  

# String Length

- Kiểm tra chuỗi có bao nhiêu ký tự sử dụng thuộc tính **length()**.
- Cú pháp 
```js
const example = 'this is a string'
console.log(example.length)
// kết quả trả về sẽ là độ dài kỹ tự của string
```
# Revising String

- Các chuỗi có chức năng tích hợp cho phép bạn kiểm tra và thao tác với nội dung của chúng.
- Đôi khi chúng ta cần thay đổi các nội dung của một chuỗi, vậy để thay đổi nội dung trong một chuỗi thì ta sử dụng phương thức **replace()**
- Cú pháp 
```js
let example = 'example string'
example = example.replace('string','this is a string')
console.log(example)
// kết quả trả về sẽ là 'example this is a string'
```
# Number

- Không giống như String, Number không cần phải viết trong đấu ngoặc đơn hay ngoặc kép 
- Number có thể là số nguyên (1,2,3,...) hoặc là số thập phân (3.14,...)

# Rounding Number

- Chúng ta có thể làm các phép toán cơ bản bằng cách sử dụng các toán tử +, -, *, / và %.
- Nhưng đối với các phép toán phức tạp hơn, chúng ta có thể sử dụng đối tượng **Math**
- Dùng **Math** để làm tròn số
```js
const roundUp = 1.5;
const rounded = Math.round(roundUp);
console.log(rounded);
// kết quả trả về giá trị của roundUp sẽ bằng 2
```
# Number To String

- Để chuyển một số thành một chuỗi sử dụng phương thức **toString()**
- Phương thức toString() là một phương thức tích hợp sẵn của đối tượng JavaScript Number nó cho phép bạn chuyển đổi bất kỳ giá trị kiểu **number** thành kiểu biểu diễn **string** của nó.
- Ví dụ
```js
var number = 128;
var str = number.toString();
console.log(str);

// "128"
```
# If Statement

- Các câu lệnh điều kiện được sử dụng để thay đổi luồng điều khiển của một chương trình,
  dựa trên một điều kiện boolean được chỉ định.
- Một câu lệnh điều kiện có dạng như sau
```js
if(n> 1) {
    console.log ('biến n lớn hơn 1.')
}else {
    console.log ('biến n nhỏ hơn hoặc bằng 1.')
    }
// (n>1): Bên trong dấu ngoặc là kết quả của lệnh sẽ là đúng hoặc sai 
// else: là lệnh tùy chọn và chứa mã sẽ được thực thi nếu kết quả đó là sai 
```
# For loop

- Vòng lặp **for** cho phép chạy lặp lại một khối mã với một số lần nhất định.
```js
for(let i = 0; i < n; i++){
    // do something
}
// let i = 0: Khởi tạo biến cho vòng lặp 
// i < n: Điều kiện để vòng lặp for thực hiện 
// i++: Tăng một giá trị mỗi khi khối mã trong vòng lặp được thực thi. 
```
# Array

- **Array** là một biến đơn được sử dụng để lưu trữ các phần tử của các kiểu dữ liệu khác nhau để chúng có thể được truy cập thông qua một biến duy nhất.
- Có thể tạo mạng bằng 2 cách 
- Cú pháp
```js
// []
const array_name = [item1, item2, ...]; 
```
```js
// new Array()
const array_name = new Array(item1, item2, ...); 
```
- Ví dụ: 
```js
const array = ['a', 'b', 'c'];
```
```js
const number = new Array(20,30,40,50);
```
# Array Filtering

- Để thực hiện lọc mạng ta sử dụng phương thức **filter()**
- Ví dụ
```js
    const array = ['a', 'b', 'c'];

    const arrays = array.filter(function (array) {
       return (array !== 'c');
    })
    console.log(arrays);
    // kết quả trả về trong array chỉ còn 'a' và 'b'
```

# Accessing Array Values 

- Các phần tử của mảng có thể được truy cập thông qua index number.
- Index number bắt đầu từ 0 đến độ dài thuộc tính của mảng trừ đi một.
- Các phần tử của mảng phải được truy cập chỉ thông qua ký hiệu dấu ngoặc.
- Ví dụ
```js
const pets = ['cat', 'dog', 'rat'];

console.log(pets[0]);
// Đoạn mã trên sẽ in ra phần tử đầu tiên của mảng pest là cat.
```
# Looping through arrays

- Sử dụng vòng lặp for để truy cập và thao tác một danh sách của các giá trị trong một mạng.
- Truy cập các giá trị của mảng có thể được thực hiện bằng cách sử dụng một số nguyên.
- Mỗi mục trong một mảng được xác định bằng một số, bắt đầu từ số 0
- Ví dụ
```js
const pest = ['cat','dog','rat']
for(let i = 0; i < pest.length; i++){
    pest[i] = pest[i] + 's'
}
console.log(pest)
// => [ 'cats', 'dogs', 'rats' ]
// Thay đổi từng chuỗi để chúng là số nhiều
```

# Object

- **Object** là danh sách các giá trị tương tự mảng, ngoại trừ các giá trị được xác định bằng các key thay vì số nguyên.

# Object Properties

- Bạn có thể truy cập và thao tác các thuộc tính của đối tượng, các khóa và giá trị mà một đối tượng chứa, sử dụng một phương thức rất giống với mạng
- Ví dụ
```js
const food = {
types:'only pizza'
}
console.log(food.types)
// => only pizza
```

# Object keys

- Javascript cung cấp một cách liệt kê nguyên bản tất cả các khóa có sẵn của một đối tượng. Điều này giúp cho việc lặt qua tất cả các thuộc tính của một đối tượng và thao tác tất cả các giá trị của chúng cho phù hợp.
- Để liệt kê tất cả các khóa đối tượng bằng cách sử dụng **Object.keys()**
- Ví dụ
```js
const car = {
    make: 'Toyota',
    model: 'Camry',
    year: 2022
    }
const keys = Object.keys(car);
console.log(keys);

// => [ 'make', 'model', 'year' ]
```

# Functions

- **Functions** là một khối nhận đầu vào, xử lý đầu vào đó và sau đó sản xuất đầu ra. 

# Function Arguments

- Function có thể được khai báo để nhận bất kỳ số lượng đối số nào.
- Các đối số có thể thuộc bất kỳ loại nào. 
- Một đối số có thể là một số, một chuỗi, một mảng, một đối tượng và thậm chí một chức năng khác 
- Ví dụ
```js
function math (a,b,c){
    return((b * c) + a)
}
console.log(math(53,61,67))
// 4140
```
# SCOPE 

- **Scope** là tập hợp các biến, đối tượng và hàm mà bạn có quyền được truy cập 
- Javascript có 2 scope: **global** và **local**
- Biến được khai báo bên ngoài định nghĩa hàm là một biến toàn cục và giá trị của nó có thể truy cập và sửa đội được trong suốt chương trình.
- Biến được khai báo bên trong đinh nghĩa hàm là một biến cục bộ, nó được tạo và hủy mỗi khi hàm được thực thi, và nó không thể được truy cập bởi bất kỳ mã nào bên ngoài hàm.
- Các hàm được định nghĩa bên trong các hàm khác, được gọi là các hàm lồng nhau, có thể truy cập vào phạm vi chức năng mẹ của chúng.
- Ví dụ
```js
const a = 4 // a là một biến toàn cục, nó có thể được truy cập bằng các hàm bên dưới

function foo () {
const b = a * 3 // b không thể được truy cập bên ngoài hàm foo, nhưng có thể được truy cập bởi các hàm
// được định nghĩa bên trong foo
function bar (c) {
    const b = 2 // một biến `b` khác được tạo bên trong phạm vi hàm bar
    // các thay đổi đối với biến `b` mới này không ảnh hưởng đến biến` b` cũ
    console.log (a, b, c)
}
bar(b * 4)
}

foo () // 4, 2, 48
```
-  IIFE, Immediately Invoked Function Expression, là một mẫu phổ biến cho tạo local spcope
```js
(function () {// biểu thức hàm được bao quanh bởi dấu ngoặc
// các biến được xác định ở đây
// không thể truy cập bên ngoài
}) () // hàm ngay lập tức được gọi
```
- Ví dụ
```js
   const a = 1; const b = 2; const c = 3;

    (function firstFunction () {
       const b = 5; const c = 6;
       (function secondFunction () {
        const b = 8;
        console.log(`a: ${a}, b: ${b}, c: ${c}`);
       })()
    })()
// => a = 1; b = 8; c = 6 
```