## 🛠️ Development

### Available Commands

| Command | Description |
|---------|-------------|
| `bun dev` | Start development server |
| `bun build` | Build for production |
| `bun typecheck` | Check TypeScript types |
| `bun lint` | Run ESLint + Stylelint |
| `bun test:ut` | Run unit tests |
| `bun test:coverage` | Generate test coverage |

### Layer-specific Commands
```bash
# Work with specific layers
bun --filter vket-boilerplate-nuxt-base dev
bun --filter vket-boilerplate-nuxt-main build
bun --filter vket-boilerplate-nuxt-showcases test:ut
```

### Component Development

#### Naming Convention
- `Ha*` - Atoms (HaButton, HaInput)
- `Hm*` - Molecules (HmLoginForm, HmProductCard) 
- `Ho*` - Organisms (HoHeader, HoProductList)
- `Ht*` - Templates (HtTopPage, HtProductPage)

#### Component Structure
```vue
<template>
  <div :class="['hm-component', `-${variant}`]">
    {{ i18n.t('title') }}
  </div>
</template>

<i18n lang="yaml">
ja:
  title: タイトル
en:
  title: Title
</i18n>

<script lang="ts">
export default defineComponent({
  name: 'HmComponent',
})
</script>

<script setup lang="ts">
const props = withDefaults(
  defineProps<{
    variant?: 'primary' | 'secondary'
  }>(),
  {
    variant: 'primary',
  },
)

const i18n = useI18n()
</script>
```

## 🧪 Quality Assurance

### Required Checks
Before committing, ensure all these pass:
```bash
bun typecheck  # Must be 0 TypeScript errors
bun lint       # Must be 0 lint errors  
bun test:ut    # All tests must pass
```

### Git Hooks
- **Pre-commit**: Automatically runs lint-staged
- **Commit-msg**: Enforces conventional commit format

## 🌐 Internationalization

All components must include i18n blocks:
```vue
<i18n lang="yaml">
ja:
  welcome: ようこそ
  description: これは説明です
en:
  welcome: Welcome
  description: This is a description
</i18n>
```

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



## 🛠️ 開発

### 利用可能コマンド

| コマンド | 説明 |
|---------|-------------|
| `bun dev` | 開発サーバー起動 |
| `bun build` | 本番用ビルド |
| `bun typecheck` | TypeScript型チェック |
| `bun lint` | ESLint + Stylelint実行 |
| `bun test:ut` | ユニットテスト実行 |
| `bun test:coverage` | テストカバレッジ生成 |

### レイヤー固有コマンド
```bash
# 特定レイヤーでの作業
bun --filter vket-boilerplate-nuxt-base dev
bun --filter vket-boilerplate-nuxt-main build
bun --filter vket-boilerplate-nuxt-showcases test:ut
```

## 🧪 品質保証

### 必須チェック
コミット前に以下が全て通ることを確認：
```bash
bun typecheck  # TypeScriptエラー0件必須
bun lint       # lintエラー0件必須
bun test:ut    # 全テスト成功必須
```

## 🌐 国際化

全コンポーネントはi18nブロックを含める必要があります：
```vue
<i18n lang="yaml">
ja:
  welcome: ようこそ
  description: これは説明です
en:
  welcome: Welcome  
  description: This is a description
</i18n>
```

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
