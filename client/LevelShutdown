#LevelShutdown

open client.dll
press `shift+F12` and search `map_shutdown`
go to the first xref and decompile, here is your levelshutdown function.

```c
  __int64 sub_180B9A200()
{
  __int64 v0; // rax

  v0 = (*(__int64 (__fastcall **)(__int64, const char *, _QWORD, _QWORD))(*(_QWORD *)qword_182550E00 + 48LL))(
         a1: qword_182550E00,
         a2: "map_shutdown",
         a3: 0,
         a4: 0);
  if ( v0 != 0 )
    (*(void (__fastcall **)(__int64, __int64))(*(_QWORD *)qword_182550E00 + 64LL))(a1: qword_182550E00, a2: v0);
  return sub_180BA7DF0();
}
```

current pattern is `48 83 EC 28 48 8B 0D ? ? ? ? 48 8D 15 ? ? ? ? 45 33 C9 45 33 C0 48 8B 01 FF 50 30 48 85 C0 74 ? 48 8B 0D ? ? ? ? 48 8B D0 4C 8B 01 41 FF 50 40 48 83 C4 28`
