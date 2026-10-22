# Monster Clash · Kho ảnh linh thú

Kho ảnh gốc (độ phân giải cao, chưa nén) của linh thú, động tác và hiệu ứng. Code game nằm ở repo `monsterclash`. Repo này chỉ chứa ảnh nguồn.

## Cấu trúc

```
linh-thu/<mã>-<tên>/
  master_goc.png         ảnh gốc từ ChatGPT, nền trắng
  master.png             đã tách nền, 1024×1024, quay mặt sang phải
  pose/<động tác>.png    idle, attack, hit, faint, power, run, jump, dash (nền trắng)
  cutin.png              cận mặt khi tung Special
  chieu/fx_<chiêu>.png   hiệu ứng chiêu riêng (nền đen)
  tuyet-chieu/charge.png, impact.png   tuyệt chiêu phủ kín màn hình 16:9
hieu-ung-chung/          hào quang, tia nổ, thủ thế, phản đòn, hồi máu, vệt tốc độ, đất nứt
manifest.json            danh sách mọi file kèm ghi chú
```

## Quy tắc thêm ảnh mới
- Lưu ảnh từ ChatGPT vào đúng thư mục của linh thú và **đổi tên theo cấu trúc trên** trước khi đưa lên repo, ví dụ `linh-thu/B02-emberlynx/pose/attack.png`.
- Tên ảnh chiêu lấy đúng tên file trong trang Chiêu Thức, ví dụ `chieu/fx_ember_claws.png`.
- Không cần tách nền hay thu nhỏ. Claude tự xử lý khi đưa vào game.
- Linh thú chưa có thư mục thì tạo mới theo mẫu `<mã>-<tên viết thường>`, ví dụ `B03-magmutt`.

## Tình trạng

| Mã | Linh thú | Hệ | Master | Pose | Cut-in | Chiêu riêng | Tuyệt chiêu |
|---|---|---|---|---|---|---|---|
| A01 | Lampyx | Lửa | ✔ | 8/8 | ✔ | 3 | ✔ |
| A02 | Mudgo | Nước | ✔ | 8/8 | ✔ | 3 | ✔ |
| A03 | Saolet | Cỏ | ✔ | 8/8 | ✔ | 4 | ✔ |
| B02 | Emberlynx | Lửa | ✔ | 0/8 | — | — | — |
| B04 | Pyrohorn | Lửa | ✔ | 0/8 | — | — | — |
| B05 | Ashwing | Lửa/Gió | ✔ | 0/8 | — | — | — |
| B03 | Magmutt | Lửa/Đá | — | 0/8 | — | — | — |
| B23 | Flintail | Đá/Lửa | ✔ | 0/8 | — | — | — |
| B21 | Pebblit | Đá | ✔ | 0/8 | — | — | — |
| B22 | Cragox | Đá | ✔ | 0/8 | — | — | — |
| B24 | Geodillo | Đá | — | 0/8 | — | — | — |
| B06 | Brooklet | Nước | ✔ | 0/8 | — | — | — |
| B07 | Shellfin | Nước | ✔ | 0/8 | — | — | — |
| B08 | Riptalon | Nước | — | 0/8 | — | — | — |
| B09 | Mistwhale | Nước/Gió | — | 0/8 | — | — | — |
| B10 | Abysscale | Nước/Bóng tối | — | 0/8 | — | — | — |
| B31 | Frostkit | Băng | ✔ | 0/8 | — | — | — |
| B34 | Snowmote | Băng | ✔ | 0/8 | — | — | — |
| B32 | Glacibear | Băng/Đá | — | 0/8 | — | — | — |
| B12 | Thornbuck | Cỏ/Đá | — | 0/8 | — | — | — |
| B13 | Mossback | Cỏ | — | 0/8 | — | — | — |
| B14 | Bloomantis | Cỏ | ✔ | 0/8 | — | — | — |
| B15 | Vinewarden | Cỏ | — | 0/8 | — | — | — |
| B25 | Ironroot | Cỏ/Đá | — | 0/8 | — | — | — |
| B45 | Dusksnake | Độc/Bóng tối | ✔ | 0/8 | — | — | — |
| B46 | Venomantis | Độc | ✔ | 0/8 | — | — | — |
| B42 | Brambleboar | Thường/Cỏ | — | 0/8 | — | — | — |
| B16 | Voltkit | Điện | ✔ | 0/8 | — | — | — |
| B17 | Coilpup | Điện | ✔ | 0/8 | — | — | — |
| B18 | Stormhorn | Điện/Gió | — | 0/8 | — | — | — |
| B19 | Sparkfinch | Điện/Gió | — | 0/8 | — | — | — |
| B20 | Thunderjaw | Điện/Đá | — | 0/8 | — | — | — |
| B26 | Zephlet | Gió | — | 0/8 | — | — | — |
| B27 | Galegriff | Gió | — | 0/8 | — | — | — |
| B28 | Cloudkip | Gió | ✔ | 0/8 | — | — | — |
| B36 | Dustrunner | Đá | — | 0/8 | — | — | — |
| B37 | Dunehorn | Đá | — | 0/8 | — | — | — |
| B38 | Burrowbit | Đá | — | 0/8 | — | — | — |
| B39 | Sunscarab | Đá | — | 0/8 | — | — | — |
| B40 | Sandmaw | Đá/Bóng tối | — | 0/8 | — | — | — |
| B33 | Icetalon | Băng/Gió | — | 0/8 | — | — | — |
| B35 | Borealisk | Băng/Bóng tối | — | 0/8 | — | — | — |
| B29 | Skyrake | Gió/Đá | — | 0/8 | — | — | — |
| B47 | Nightpurr | Bóng tối | — | 0/8 | — | — | — |
| B48 | Gloomfang | Bóng tối | ✔ | 0/8 | — | — | — |
| B49 | Cryptowl | Bóng tối/Gió | ✔ | 0/8 | — | — | — |
| B50 | Umbrawyrm | Bóng tối/Đá | — | 0/8 | — | — | — |
| B41 | Nibblet | Thường | — | 0/8 | — | — | — |
| B43 | Pouchimp | Thường | ✔ | 0/8 | — | — | — |
| B44 | Shellpanda | Thường/Đá | ✔ | 0/8 | — | — | — |
| B30 | Tempestrix | Gió/Điện | — | 0/8 | — | — | — |

Ba linh thú khởi đầu (A01–A03) đã đủ bộ. Các linh thú mã B hiện mới có ảnh master, prompt cho phần còn lại nằm trong trang Chiêu Thức.
