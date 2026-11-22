# FlashOverlay

open client.dll
press `shift+F12` and search `FlashbangOverlay`
go to the first xref and decompile.

```c
                v21 = 0;
        v22 = v20(a1: a3, a2: "FlashbangOverlay", a3: a5, a4: v21, a5: v43, a6: 0); // you are here
        v23 = *(_DWORD *)(v22 + 60);
```

go to the top
```c
void __fastcall sub_1811DE280(__int64 a1, int a2, __int64 *a3, __int64 a4, __m128 *a5) // -> FlashOverlay
{
  __int64 v6; // r15
  int v8; // r13d
```

sub_1811DE280 is our function

current pattern is `85 D2 0F 88 ? ? ? ? 48 89 4C 24 ? 55 56`
