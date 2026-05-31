◆VSCodeでプッシュするものの「GitHubで"VitalTeamC/VitalSmartGreen"にプッシュするためのアクセス許可がありません。代わりに、フォークを作成してそれにプッシュしますか？」と表示される。

PS E:\取り組み\VitalSmartGreen> git remote set-url origin git@github.com:VitalTeamC/VitalSmartGreen.git
PS E:\取り組み\VitalSmartGreen> git remote -v
origin  git@github.com:VitalTeamC/VitalSmartGreen.git (fetch)
origin  git@github.com:VitalTeamC/VitalSmartGreen.git (push)
PS E:\取り組み\VitalSmartGreen> git push origin HEAD
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 289 bytes | 289.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:VitalTeamC/VitalSmartGreen.git
   7b96616..2e98d56  HEAD -> main
PS E:\取り組み\VitalSmartGreen> 