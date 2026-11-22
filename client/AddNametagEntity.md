# AddNametagEntity

open client.dll
press `shift+F12` and search `Nametag: %s`
go to the first xref and decompile, here is your function.

```c
      if ( *(_QWORD *)(v10 + 32) != 0 )
        v11 = *(const char **)(v10 + 32);
      CUtlString::Format(this: (CUtlString *)&v131, a2: "Nametag: %s", v11); // you are here
      v8 = v131;
```

go to the top
```c
char __fastcall sub_180802B00(__int64 a1, __int64 a2)
{
  const char *v5; // r12
  __int64 v6; // rdi
```

sub_180802B00 is our function

current pattern is `40 55 53 56 48 8D AC 24 ? ? ? ? 48 81 EC ? ? ? ? 48 8B DA`
