## 🔧 Configuration

### Environment Variables
```bash
# .env.local
VITE_OUTPUT_ENV=local  # local/staging/production
```

### Layer Configuration
Each layer has its own:
- `nuxt.config.ts` - Nuxt configuration
- `package.json` - Dependencies and scripts
- `tsconfig.json` - TypeScript configuration

## 🤝 Contributing

1. **Read the guidelines**: Check [`AGENTS.md`](./AGENTS.md) for development standards
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Follow the code style**: Use the established patterns
4. **Add tests**: Cover your changes with tests
5. **Run quality checks**: Ensure all checks pass
6. **Submit PR**: Use the provided PR template

### Commit Convention
```
[layer/scope] type: description

- What: Brief description of changes
- Why: Reason for the change  
- How: Implementation approach (if complex)
```

Examples:
- `[base/components] feat: add HmDataTable component`
- `[main/pages] fix: resolve navigation issue in mobile view`
## 📚 Documentation

- [`AGENTS.md`](./AGENTS.md) - Complete development guide for AI agents
- [`repomix-output.md`](./repomix-output.md) - Full codebase structure
- [Nuxt Docs](https://nuxt.com/docs) - Framework documentation
- [Zod Docs](https://zod.dev) - Schema validation
- [RSCSS](https://rscss.io) - CSS naming convention


## 🤝 コントリビューション

1. **ガイドラインを読む**: 開発標準について[`AGENTS.md`](./AGENTS.md)を確認
2. **フィーチャーブランチ作成**: `git checkout -b feature/amazing-feature`
3. **コードスタイルに従う**: 確立されたパターンを使用
4. **テストを追加**: 変更にテストを追加
5. **品質チェック実行**: 全チェックが通ることを確認
6. **PR提出**: 提供されたPRテンプレートを使用


### コミット規約

```
[layer/scope] type: description

- What: 変更内容の簡潔な説明
- Why: 変更の理由  
- How: 実装方法（複雑な場合のみ）
```

例：

* `[base/components] feat: HmDataTableコンポーネントを追加`
* `[main/pages] fix: モバイル表示のナビゲーション問題を修正`

## 📚 ドキュメント

* [`AGENTS.md`](./AGENTS.md) - AIエージェント開発の完全ガイド
* [`repomix-output.md`](./repomix-output.md) - コードベース全体の構造
* [Nuxt Docs](https://nuxt.com/docs) - フレームワークの公式ドキュメント
* [Zod Docs](https://zod.dev) - スキーマバリデーションのドキュメント
* [RSCSS](https://rscss.io) - CSS命名規則