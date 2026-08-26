# git-team-YutoUchima
enpit


## Task1

% git checkout -b dev-anna main && git checkout -b dev-ben main && git checkout -b dev-you main

    Switched to a new branch 'dev-anna'
    Switched to a new branch 'dev-ben'
    Switched to a new branch 'dev-you'

% ls .git/refs/heads/ && cat .git/refs/heads/dev-anna .git/refs/heads/dev-ben .git/refs/heads/dev-you


    ファイル数は4つ
    dev-anna	dev-ben		dev-you		main

    3つのファイルのSHAは同じ。
    なぜ？
    これらのブランチが作成された後、それぞれのブランチ上でまだ新しいコミットが一度も行われていない状態であるため。
    0ca3b46381b08cb3dfd37dd8e782118e33ed17da
    0ca3b46381b08cb3dfd37dd8e782118e33ed17da
    0ca3b46381b08cb3dfd37dd8e782118e33ed17da


# PartA

## Task2

% git log --oneline --graph --all

    * 54adfc8 (HEAD -> dev-you) feat: add signup feature
    | * 4d2700c (dev-ben) feat: add dark theme
    |/  
    | * 5670856 (dev-anna) feat: add login feature
    |/  
    * 0ca3b46 (origin/main, origin/HEAD, main) Initial commit

    3つのボランチが共通の初期コミット（0ca3b46）からそれぞれ独立して並行して枝分かれしている状態を表している。
