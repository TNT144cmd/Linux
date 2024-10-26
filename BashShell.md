## run bash shell: (test.sh)
./test.sh

## Cấp quyền cho file:
- chmod: 744, 777,... Check trên: [https://chmod-calculator.com/]
  VD: chmod 744 test.sh
- Check quyền của file: ls -l 

## Biến:
  Name= "Nhan"  // không được có dấu cách chỗ "Name="
  echo "Hello ${Name}
  exit 0

## Ngắt chuỗi:
  ${parameter:offset:length}

VD:
  enum=123456789
  echo ${enum:1:5}
=> 23456
  echo ${enum:5}
=> 6789
  echo ${enum::5}
=> 12345
  echo ${enum: -3:2}
  //case này đếm từ cuối đếm về// có 1 dấu cách chỗ offset
=> 78
  echo ${enum: -3}
=> 789
## run bash shell: (test.sh)
./test.sh

## Cấp quyền cho file:
- chmod: 744, 777,... Check trên: [https://chmod-calculator.com/]
  VD: chmod 744 test.sh
- Check quyền của file: ls -l 

## Biến:
 VD:
  Name= "Nhan"  // không được có dấu cách chỗ "Name="
  echo "Hello ${Name}
  exit 0

## Ngắt chuỗi:
  ${parameter:offset:length}

 VD:
  enum=123456789
  echo ${enum:1:5}
=> 23456
  echo ${enum:5}
=> 6789
  echo ${enum::5}
=> 12345
  echo ${enum: -3:2}
  //case này đếm từ cuối đếm về// có 1 dấu cách chỗ offset
=> 78
  echo ${enum: -3}
=> 789
## Variable
  VD: 
    Currentdir= $(pwd)
    echo "path: $Currendir" // show ra đường dẫn hiện tại
    exit 0
## Tính toán:
  - ${parameter}
  - $(command)
  - $((expression))
    VD:
        x= 12
        y= 5
        echo $(($x + $y))
        exit 0
  - bc để lấy số thập phân, scale=n
    VD:
        echo "scale=2; 5/2" | bc
## Range
  echo {1,2,4,nhan}
  => 1 2 4 nhan
  echo {1..5}
  => 1 2 3 4 5
  echo {a..g}
  => a b c d e f g
  echo {1..10..2}
  => 1 3 5 7 9
  echo Count{1..6..2}
  => Count1 Count3 Count5

## Special pramameter
  $0: tên chính script file đang chạy
  $*: chứa tất cả tham số được đưa vào script, nó được xem như một chuỗi chứa tất cả
  $@: chứa tất cả tham số nhưng phân thành các số riêng lẻ
  $?: trạng thái thoát ra của lệnh ngay trước đó được chạy
  $$: Số tiến trình (processID) của shell hiện tại. 
    


