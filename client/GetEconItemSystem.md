# GetEconItemSystem

open client.dll
press `shift+F12` and search `desc_attrib_neutral`
go to the first xref and decompile, here is your function.

```c
  dword_182258380 = *(_DWORD *)(*(_QWORD *)(sub_1811A0320() + 8) + 52LL);
  qword_182258388 = (__int64)"desc_attrib_neutral"; // you are here
  v8 = sub_1811A0320();
```

go to the top
```c
__int64 sub_18011C7F0()
{
  __int64 v0; // rax
  char *v1; // r14
```

sub_18011C7F0 is our function

current pattern is `E8 ? ? ? ? 4C 8B 35 ? ? ? ? 33 DB`
