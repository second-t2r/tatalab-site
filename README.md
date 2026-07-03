# TaTaLab（たたらぼ）単独サイト

second-site から**完全に独立**した TaTaLab 専用の公開用リポジトリ。

- 生成元: `~/work/second/docs/20260703_tatalab-lp_v1.html`
- ビルダ: `~/work/second/code/build_tatalab_deploy.py`（`build_lp_deploy.py` とは非共有）
- 再生成: `python3 code/build_tatalab_deploy.py`（このリポの中身＝生成物。直接編集しない）

## 状態
- 独立PWゲート（PW `tatalab`・sessionStorageキー `tatalab_gate`＝moteki と別ロック）
- noindex（robots メタ＋robots.txt）／TaTaLab専用 OGP・favicon
- **未公開**。実公開（PWゲート撤廃）は TATEITO 取締役会の競業承認後（G3）

## 公開手順（多々良・push=YELLOW / 認証=多々良のみ）
1. GitHub で空リポを作成（例: `second-t2r/tatalab-site`）
2. remote 追加: `git remote add origin git@github-second:second-t2r/tatalab-site.git`
3. `git push -u origin main`
4. GitHub Pages を有効化（Settings → Pages → Branch: main / root）
5. 独自ドメイン確定後に CNAME を追加（tatalab 系ドメインは別タスクで取得）
