# Linux

1: $(wildcard *.c): gọi các file .c trong folder

2: $(patsubst %.c, %.o, $(wildcard *.c)): thay thế các file .c thành file .o
   $(patsubst pattern, replacement, text): tìm trong text các file ứng với pattern và thay vào trong replacement

3: $@: tênc của target
  $<: tên của prerequisite đầu tiên
  $^: tên của all prequisite
