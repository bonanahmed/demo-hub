# demo-hub

> [Demo] Halaman daftar semua demo di demo.adnan-ahmad.com — Vercel rewrites
>
> GitHub topics: `fastwork-demo` `portfolio` `vercel`

Satu domain untuk semua demo. Setiap demo tetap repo + project Vercel sendiri; hub ini meneruskan path ke sana.

| Path | Repo | Project Vercel |
|---|---|---|
| `/patreon-gatekeeper` | `demo-patreon-gatekeeper` | demo-patreon-gatekeeper.vercel.app |
| `/ai-agent-kopisenja` | `demo-ai-agent-kopisenja` | demo-ai-agent-kopisenja.vercel.app |

## Menambah demo baru
1. Buat repo `demo-<nama>` dan deploy ke Vercel.
2. **Aplikasinya harus mendukung sub-path** `/<nama>`: semua link dan redirect memakai prefix (atau hanya link relatif untuk situs statis).
3. Tambah dua baris rewrite di `vercel.json` (path tanpa dan dengan `/:path*`).
4. Tambah satu kartu di `index.html`.

Path = nama repo tanpa prefix `demo-`.
