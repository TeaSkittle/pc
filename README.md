# pc
Perl Calculator

This is a very simple calculator meant for programmers. It evaluates expressions and calculates the answers in decimal, hexadeciaml, and in binary. Was inspired by [pcalc](https://vapier.github.io/pcalc/) and is written in a small amount of perl code. Can be ran as a simple interactive calculator(similar to [bc](https://www.gnu.org/software/bc/)), and can also evaluate an expression as an argument. Using redirection and tools such as xargs, pc can be useful in scripts as well.

Exmaples:
```Bash
tea@navi ~/WIP> ./pc
23 + 0x78
	143			0x8f			0b10001111
0b101
	5			0x5			0b101
exit
tea@navi ~/WIP> ./pc "6 + 0x1234 % 0b100000"
	26			0x1a			0b11010
tea@navi ~/WIP> date | awk '{print $3}' | ./pc
	14			0xe			0b1110
tea@navi ~/WIP>
```

To run, all you need to do is make pc executable:
```Bash
tea@navi ~/WIP> chmod +x pc
```
