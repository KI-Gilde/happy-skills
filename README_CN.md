# Happy Skills

**中文** | [English](./README.md)

**用自然语言描述需求，自动生成设计文档并逐步实现代码。** 把"想法→设计→代码→提交"的完整开发流程自动化。

## 安装

### 使用 npx skills（推荐）

```bash
# 安装此包中的所有 skills
npx skills add notedit/happy-skills

# 仅安装特定的 skills
npx skills add notedit/happy-skills --skills feature-dev,feature-analyzer

# 全局安装（在所有项目中可用）
npx skills add notedit/happy-skills -g
```

> **注意**: `npx skills` 需要 [skills CLI](https://www.npmjs.com/package/skills)。如果尚未安装，请运行 `npm install -g skills`。

### 验证安装

```bash
# 测试 skill
/feature-dev 添加一个简单功能

# 或者测试其他 skill
/feature-analyzer 设计用户认证系统
```

## Usage

### 1. Feature Development (Design → Execute)

```bash
# Step 1: 设计 - Q&A 对话生成设计文档
/feature-analyzer 用户登录功能，支持 OAuth2

# Step 2: 执行 - 按文档逐项实现
/feature-pipeline docs/features/user-login.md
```

### 2. Quick Development

```bash
/feature-dev 添加深色模式切换
```

### 3. Screenshot Analysis

```bash
/screenshot-analyzer ./app.png  # 从截图提取功能生成任务
```

## Components

### Skills

| Skill | Description |
|-------|-------------|
| `feature-dev` | 引导式功能开发，深入理解代码库并专注架构设计 |
| `feature-analyzer` | Turn ideas into designs through Q&A dialogue |
| `feature-pipeline` | Execute tasks from design documents |
| `screenshot-analyzer` | Extract features from UI screenshots |
| `skill-creation-guide` | Guide for creating new skills |
| `tts-skill` | MiniMax TTS API - 文本转语音、声音克隆、声音设计 |
| `react-animation` | ReactBits 动画组件 + Remotion - 精选视觉效果用于视频制作 |
| `gsap-animation` | GSAP + Remotion 动态图形 - 时间线编排、文字拆分、SVG 形变、高级缓动 |
| `video-producer` | 端到端 Remotion 视频制作 - 从自然语言描述到完整视频，叙事结构、场景编排、渲染管线 |

## Project Structure

```
happy-skills/
├── package.json                 # NPM 包配置 & skills 配置
├── skills/                      # Skills
└── docs/                        # Documentation
```

## License

MIT
