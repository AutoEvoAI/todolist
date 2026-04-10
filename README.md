<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Star Todo Pro</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            line-height: 1.8;
            color: #333;
            background: #fafafa;
        }
        .lang-toggle {
            position: fixed;
            top: 20px;
            right: 20px;
            background: #333;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 14px;
        }
        .lang-toggle:hover { background: #555; }
        h1 { color: #1a1a2e; border-bottom: 3px solid #4facfe; padding-bottom: 10px; }
        h2 { color: #2d3748; margin-top: 40px; }
        h3 { color: #4a5568; }
        code { background: #e2e8f0; padding: 2px 8px; border-radius: 4px; font-size: 0.9em; }
        pre { background: #1a1a2e; color: #fff; padding: 20px; border-radius: 12px; overflow-x: auto; }
        pre code { background: none; padding: 0; }
        ul { padding-left: 20px; }
        li { margin: 8px 0; }
        .badge {
            display: inline-block;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 12px;
            margin-right: 8px;
        }
        .badge-primary { background: #4facfe; color: white; }
        .badge-success { background: #48bb78; color: white; }
        .feature-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 20px 0; }
        .feature-card { background: white; padding: 20px; border-radius: 12px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        .feature-card h3 { margin-top: 0; color: #4facfe; }
        .divider { border: none; border-top: 1px solid #e2e8f0; margin: 40px 0; }
        hr { border: none; border-top: 1px solid #e2e8f0; margin: 40px 0; }
        .lang-content { display: none; }
        .lang-content.active { display: block; }
        footer { margin-top: 60px; padding-top: 20px; border-top: 1px solid #e2e8f0; text-align: center; color: #666; }
    </style>
</head>
<body>
    <button class="lang-toggle" onclick="toggleLang()">🌐 <span id="langLabel">中文</span></button>

    <!-- English Content -->
    <div class="lang-content active" id="en">
        <h1>🌟 Star Todo Pro</h1>
        <p><strong>A beautiful and practical todo list app with Pomodoro timer.</strong></p>
        
        <p>
            <span class="badge badge-primary">v1.0.0</span>
            <span class="badge badge-success">MIT License</span>
        </p>

        <h2>✨ Features</h2>
        <div class="feature-grid">
            <div class="feature-card">
                <h3>📝 Task Management</h3>
                <p>Add, complete, and delete todos with ease</p>
            </div>
            <div class="feature-card">
                <h3>🍅 Pomodoro Timer</h3>
                <p>25-minute focus timer to boost productivity</p>
            </div>
            <div class="feature-card">
                <h3>⏱️ Time Tracking</h3>
                <p>Track time spent on each task</p>
            </div>
            <div class="feature-card">
                <h3>💾 Data Persistence</h3>
                <p>All data saved locally with localStorage</p>
            </div>
            <div class="feature-card">
                <h3>🌌 Beautiful Design</h3>
                <p>Starfield theme with stunning animations</p>
            </div>
            <div class="feature-card">
                <h3>🌍 Multilingual</h3>
                <p>Supports English and Chinese with auto-detection</p>
            </div>
        </div>

        <h2>🚀 Quick Start</h2>
        <pre><code># Just open index.html in your browser
open index.html</code></pre>
        <p>No installation required. Works offline!</p>

        <h2>📖 Usage</h2>
        <ol>
            <li>Open <code>index.html</code> in any modern browser</li>
            <li>Type your task in the input box, press Enter or click "Add"</li>
            <li>Click the 🍅 button to start the Pomodoro timer</li>
            <li>Click the ✓ button to complete a task</li>
            <li>Click the 🗑️ button to delete a task</li>
            <li>Use the 🌐 button to switch language</li>
        </ol>

        <h2>🛠️ Tech Stack</h2>
        <ul>
            <li>HTML5 + CSS3 + Vanilla JavaScript</li>
            <li>No dependencies required</li>
            <li>localStorage for data persistence</li>
            <li>CSS animations for visual effects</li>
        </ul>

        <h2>🎨 Preview</h2>
        <ul>
            <li>Dark starfield background with animated stars</li>
            <li>Frosted glass effect task cards</li>
            <li>Prominent Pomodoro timer</li>
            <li>Task statistics (total pomodoros, today's count)</li>
        </ul>

        <h2>📄 License</h2>
        <p>This project is licensed under the MIT License - see the <code>LICENSE</code> file for details.</p>
        <pre><code>MIT License

Copyright (c) 2024 Star Todo Pro

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.</code></pre>

        <h2>🤝 Contributing</h2>
        <p>Contributions are welcome! Please feel free to submit a Pull Request.</p>
    </div>

    <!-- Chinese Content -->
    <div class="lang-content" id="zh">
        <h1>🌟 星空Todo Pro</h1>
        <p><strong>一个美观实用的待办事项管理应用，带有番茄钟功能。</strong></p>
        
        <p>
            <span class="badge badge-primary">v1.0.0</span>
            <span class="badge badge-success">MIT License</span>
        </p>

        <h2>✨ 功能特点</h2>
        <div class="feature-grid">
            <div class="feature-card">
                <h3>📝 任务管理</h3>
                <p>轻松添加、完成、删除待办事项</p>
            </div>
            <div class="feature-card">
                <h3>🍅 番茄钟</h3>
                <p>25分钟专注计时器，帮助提升专注力</p>
            </div>
            <div class="feature-card">
                <h3>⏱️ 时间追踪</h3>
                <p>记录每个任务花费的番茄时间</p>
            </div>
            <div class="feature-card">
                <h3>💾 数据持久化</h3>
                <p>使用 localStorage 保存所有数据</p>
            </div>
            <div class="feature-card">
                <h3>🌌 视觉效果</h3>
                <p>星空主题设计，美观的动画效果</p>
            </div>
            <div class="feature-card">
                <h3>🌍 多语言支持</h3>
                <p>支持中英文，自动检测浏览器语言</p>
            </div>
        </div>

        <h2>🚀 快速开始</h2>
        <pre><code># 直接在浏览器中打开 index.html
open index.html</code></pre>
        <p>无需安装，支持离线使用！</p>

        <h2>📖 使用方法</h2>
        <ol>
            <li>在任意现代浏览器中打开 <code>index.html</code></li>
            <li>在输入框中输入任务，按 Enter 或点击"添加"按钮</li>
            <li>点击任务右侧的 🍅 按钮启动番茄钟</li>
            <li>点击 ✓ 按钮完成任务</li>
            <li>点击 🗑️ 按钮删除任务</li>
            <li>点击 🌐 按钮切换语言</li>
        </ol>

        <h2>🛠️ 技术栈</h2>
        <ul>
            <li>HTML5 + CSS3 + 原生 JavaScript</li>
            <li>无需安装任何依赖</li>
            <li>localStorage 存储数据</li>
            <li>CSS 动画实现视觉效果</li>
        </ul>

        <h2>🎨 界面预览</h2>
        <ul>
            <li>深色星空背景，带有动态星星效果</li>
            <li>半透明毛玻璃效果的任务卡片</li>
            <li>醒目的番茄钟计时器</li>
            <li>任务统计展示（总番茄数、今日番茄数）</li>
        </ul>

        <h2>📄 许可证</h2>
        <p>本项目基于 MIT 许可证开源 - 详见 <code>LICENSE</code> 文件。</p>
        <pre><code>MIT License

版权所有 (c) 2024 Star Todo Pro

特此免费向任何获得本软件和相关文档文件（"软件"）副本的人提供，
不受限制地处理本软件，包括但不限于使用、复制、修改、合并、发布、
分发、再许可和/或出售本软件副本的权利，并允许获得本软件的人这样做，
但须满足以下条件：

上述版权声明和本许可声明应包含在本软件的所有副本或主要部分中。

本软件按"原样"提供，不提供任何形式的明示或暗示担保，包括但不限于
对适销性、特定用途适用性和非侵权性的担保。</code></pre>

        <h2>🤝 贡献</h2>
        <p>欢迎贡献代码！请随时提交 Pull Request。</p>
    </div>

    <footer>
        <p>Made with ❤️ | <a href="https://github.com/AutoEvoAI/todolist">GitHub</a></p>
    </footer>

    <script>
        let currentLang = localStorage.getItem('readme-lang') || 'en';
        
        function toggleLang() {
            currentLang = currentLang === 'en' ? 'zh' : 'en';
            localStorage.setItem('readme-lang', currentLang);
            applyLang();
        }
        
        function applyLang() {
            document.getElementById('langLabel').textContent = currentLang === 'en' ? '中文' : 'EN';
            document.querySelectorAll('.lang-content').forEach(el => {
                el.classList.remove('active');
            });
            document.getElementById(currentLang).classList.add('active');
        }
        
        applyLang();
    </script>
</body>
</html>
