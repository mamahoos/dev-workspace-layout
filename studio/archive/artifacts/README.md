# `artifacts/` — غیرسورس

| پوشه | محتوی |
| --- | --- |
| `archives/projects/` | zip/tar اسنپ‌شات پروژه |
| `archives/platforms/` | بکاپ سنگین سرویس (سرور، coolify، …) |
| `archives/generic/` | tar/zip بدون برچسب پروژه |
| `exports/` | خروجی اپ؛ کنار zip یک `unpacked/` |
| `container-images/docker-images/` | `docker save` |
| `databases/` | `.sql` / `.db` تک‌فایل (نه `.db` داخل ریپو) |
| `documents/` | سند تک‌فایل که پروژه نیست |
| `scripts/` | sh/py پراکنده |
| `config-snippets/` | قطعه کانفیگ؛ `vpn/` حساس است |

مسیر سازگاری: `archive/docker-images` → `container-images/docker-images`.
