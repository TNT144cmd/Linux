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
