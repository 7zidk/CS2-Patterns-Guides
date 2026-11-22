# CreateMove

open client.dll
press `shift+F12` and search `Original entries:\n`
go to the first xref and decompile, here is your function.

```c
      if ( (unsigned __int8)LoggingSystem_IsChannelEnabled(a1: (unsigned int)dword_1824CF680, a2: 2) != 0 )
        LoggingSystem_Log(a1: (unsigned int)dword_1824CF680, a2: 2, a3: "Original entries:\n"); // you are here 
      v75 = dword_1824CF680;
```

go to the top
```c
__int64 __fastcall sub_180D04300(__int64 a1, unsigned int a2, __int64 a3) // -> CreateMove
{
  __int64 v6; // rax
  __int64 v7; // rdx
```

sub_180D04300 is our function

current pattern is `48 8B C4 4C 89 40 ? 48 89 48 ? 55 53 57`
