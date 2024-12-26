## Seoulcomix Github Actions

#### 📥 Monorepo install

```yaml
- name: 📥 Monorepo install
  uses: seoulcomix/actions/yarn-nm-install@main
  with:
    enable-corepack: true
    cache-node-modules: true
    cache-install-state: true
    use-blacksmith: true # default: true
```

#### 📥 Next.js cache

```yaml
- name: 📥 Next.js cache
  uses: seoulcomix/actions/nextjs-cache@main
  with:
    use-blacksmith: true # default: true
```

#### 📥 Remove older drafts

```yaml
- name: 📥 Remove older drafts
  uses: seoulcomix/actions/remove-older-drafts@main
  with:
    github-repo: ${{ github.repository }}
```

#### 📥 Unstaged diff

```yaml
- name: 📥 Unstaged diff
  uses: seoulcomix/actions/unstaged-diff@main
  with:
    command: yarn lint
```
