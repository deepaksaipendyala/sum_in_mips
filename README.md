# sum_in_mips

### Addition with input
```
.data
msg1: .asciiz"Enter the num 1:"
msg2: .asciiz"Enter the num 2:"

.text
li $v0,4
la $a0,msg1
syscall
li $v0,5
syscall
move $s0,$v0

li $v0,4
la $a0,msg2
syscall
li $v0,5
syscall
move $s1,$v0

add $s2,$s0,$s1

move $a0,$s2
li $v0,1
syscall

```
