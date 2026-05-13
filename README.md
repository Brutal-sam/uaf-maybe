- Webkit Use After Free in EventTarget.
- Tested on PS5 11.20. (the crash happens on the latest fw 13.20 as well)
- exploitability not determined, this may or may not be useful.

the second run should return "A" in rax 
this is just a crash html, it doesn't attempt to control rip or leak anything.
whether it can be Exploited or not will be determined by developers 

```
# signal: 4 (SIGILL)
# thread ID: 101798
# thread name: SceNKWebProcessMain
# proc ID: 101
# proc name: SceNKWebProcess
# reason: privileged instruction fault
#
# registers:
# rax: 4141414141414141  rbx: 00000010008b1d50
# rcx: 4a0a0a09c8fb81a2  rdx: 0000000821d10cf8
# rsi: 0000001000888cc0  rdi: 00000010003e63b8
# rbp: 00000007ef0fdcb0  rsp: 00000007ef0fdb50
# r8 : 0000000000020000  r9 : 00000000004e0000
# r10: 00000000001de750  r11: 0000000821c1bb58
# r12: 0000000000000008  r13: 0000001000332d68
# r14: 00000010008f6fc0  r15: 00000010008b0040
# rip: 000000082039d566  eflags: 00010212
# lbf: 000000082039c634  lbt: 000000082039d566
# lb0: ffffffffffffffff  lb1: ffffffffffffffff
# lb2: 000000082039d566  lb3: 000000082039c5f0
# lb4: 00000008206e21a7  lb5: 00000008206e2152
# lb6: 00000008206e208c  lb7: 000000082039e632
```
