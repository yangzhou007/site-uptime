# site-uptime

每 15 分钟检查网站首页能不能打开（GitHub Actions，跑在 GitHub 服务器上）。
连续 3 次打不开才推一次微信（Server 酱，secret `SERVERCHAN_SENDKEY`），恢复时再推一次；同一次故障不重复推。
加网站：在 `.github/workflows/uptime.yml` 的 `matrix.site` 加一行。
