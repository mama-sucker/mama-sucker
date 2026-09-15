<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Addison Roy — README</title>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body {
    background: var(--background, #09090b);
    color: var(--foreground, #e4e4e7);
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    padding: 1.5rem 1rem;
    max-width: 700px;
    margin: 0 auto;
  }

  /* Terminal header */
  .terminal {
    background: #0d1117;
    border: 1px solid #1e1e24;
    border-radius: 10px;
    overflow: hidden;
    max-width: 560px;
    width: 100%;
    margin: 0 auto 1.5rem;
    box-shadow: 0 4px 24px rgba(0,0,0,0.5);
  }
  .terminal-bar {
    background: #1e1e24;
    padding: 8px 14px;
    display: flex;
    align-items: center;
    gap: 8px;
    border-bottom: 1px solid #1e1e24;
  }
  .dot { width: 10px; height: 10px; border-radius: 50%; }
  .dot.r { background: #ff5f57; box-shadow: 0 0 4px rgba(255,95,87,0.3); }
  .dot.y { background: #febc2e; box-shadow: 0 0 4px rgba(254,188,46,0.3); }
  .dot.g { background: #28c840; box-shadow: 0 0 4px rgba(40,200,64,0.3); }
  .terminal-title {
    color: #71717a;
    font-size: 11px;
    font-family: 'Courier New', monospace;
    margin-left: 8px;
  }
  .terminal-body {
    padding: 18px 22px;
    font-family: 'Courier New', monospace;
    min-height: 120px;
  }
  #term-output {
    color: #7ee787;
    font-size: 13px;
    line-height: 1.7;
    white-space: pre-wrap;
  }
  #term-cursor {
    color: #7ee787;
    animation: blink 800ms step-end infinite;
  }
  @keyframes blink {
    0%, 50% { opacity: 1; }
    51%, 100% { opacity: 0; }
  }

  /* Badges row */
  .badges {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    justify-content: center;
    margin-bottom: 1.5rem;
  }
  .badge {
    display: inline-block;
    padding: 3px 9px;
    border-radius: 4px;
    font-size: 11px;
    font-weight: 600;
    border: 1px solid;
  }

  /* Code block */
  .code-block {
    background: #0d1117;
    border: 1px solid #1e1e24;
    border-radius: 8px;
    padding: 14px 18px;
    font-family: 'Courier New', monospace;
    font-size: 13px;
    color: #7ee787;
    margin-bottom: 1.5rem;
    overflow-x: auto;
  }
  .code-block .prompt { color: #6e7681; }
  .code-block .val { color: #e4e4e7; }

  /* Sections */
  h2 {
    font-size: 1.1rem;
    font-weight: 600;
    color: #e4e4e7;
    margin-bottom: 0.6rem;
    display: flex;
    align-items: center;
    gap: 6px;
  }
  h2::before {
    content: '';
    width: 14px;
    height: 1px;
    background: #38bdf8;
  }
  p, li {
    color: #71717a;
    font-size: 13px;
    line-height: 1.7;
  }
  .section { margin-bottom: 1.5rem; }
  ul { padding-left: 18px; margin-top: 0.4rem; }
  li { margin-bottom: 4px; }
  li strong { color: #e4e4e7; font-weight: 600; }

  hr {
    border: none;
    border-top: 1px solid #1e1e24;
    margin: 1.5rem 0;
  }

  /* Tech badges */
  .tech-row {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }
  .tech {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    padding: 4px 10px;
    border-radius: 6px;
    font-size: 11px;
    font-weight: 500;
    border: 1px solid #1e1e24;
    background: #111113;
  }

  .footer {
    text-align: center;
    padding: 1.5rem 0;
    border-top: 1px solid #1e1e24;
    color: #3f3f46;
    font-size: 11px;
  }
</style>
</head>
<body>

<!-- TERMINAL BANNER -->
<div class="terminal">
  <div class="terminal-bar">
    <span class="dot r"></span>
    <span class="dot y"></span>
    <span class="dot g"></span>
    <span class="terminal-title">addison@homelab ~</span>
  </div>
  <div class="terminal-body">
    <div id="term-output"></div>
    <span id="term-cursor">█</span>
  </div>
</div>

<!-- BADGES -->
<div class="badges">
  <span class="badge" style="border-color: #006747; color: #3fb950;">🎓 USF Cybersecurity</span>
  <span class="badge" style="border-color: #557C94; color: #81a9cc;">🐧 Kali Linux</span>
  <span class="badge" style="border-color: #48B9C7; color: #66d9e7;">💜 Pop!_OS</span>
  <span class="badge" style="border-color: #E57000; color: #f09830;">📦 Proxmox</span>
  <span class="badge" style="border-color: #88171A; color: #d06060;">🔒 WireGuard</span>
</div>

<!-- CODE BLOCK -->
<div class="code-block">
  <span class="prompt">addison@homelab:~$</span> <span class="val">whoami</span><br>
  cybersecurity student @ USF | homelab operator | AI tinkerer<br><br>
  <span class="prompt">addison@homelab:~$</span> <span class="val">uname -a</span><br>
  Proxmox cluster (3 nodes) :: Dell PowerEdge R630 :: 3x RTX 5060 Ti<br><br>
  <span class="prompt">addison@homelab:~$</span> <span class="val">status</span><br>
  <span style="color:#3fb950;">[ONLINE]</span> all systems nominal, one service definitely on fire
</div>

<!-- ABOUT -->
<div class="section">
  <h2>What I'm into</h2>
  <p>
    I'm a cybersecurity student, and I like learning security concepts by actually building and breaking infrastructure rather than just reading about it. Most of that happens in my own homelab.
  </p>
  <ul>
    <li><strong>Offensive &amp; defensive practice</strong> — running a Kali Linux VM as a dedicated ops box, working through network segmentation and Zero Trust tunneling</li>
    <li><strong>Infrastructure security</strong> — self-managed Proxmox environment, including hands-on RAID recovery and cluster rebuild work</li>
    <li><strong>Applied AI</strong> — running local LLMs instead of relying on hosted APIs, partly out of interest in data control and model behavior</li>
  </ul>
</div>

<hr>

<!-- HOMELAB -->
<div class="section">
  <h2>My homelab</h2>
  <p>A three-cluster Proxmox setup that I use as a sandbox for security work, self-hosting, and AI experimentation:</p>
  <ul>
    <li><strong>Compute core:</strong> Dell PowerEdge R630 running Proxmox</li>
    <li><strong>Local LLM rig:</strong> three RTX 5060 Ti GPUs serving quantized models via vLLM / llama.cpp</li>
    <li><strong>Networking:</strong> WireGuard VPN + Cloudflare Zero Trust tunnels for secure remote access</li>
    <li><strong>Self-hosted services:</strong> Nextcloud, Jellyfin, Gitea, and various LXC containers</li>
  </ul>
</div>

<hr>

<!-- TOOLS -->
<div class="section">
  <h2>Tools &amp; tech</h2>
  <div class="tech-row">
    <span class="tech">🐧 Linux</span>
    <span class="tech">📦 Proxmox</span>
    <span class="tech">🐳 Docker</span>
    <span class="tech">🐍 Python</span>
    <span class="tech">📙 Git</span>
    <span class="tech">📜 Bash</span>
  </div>
</div>

<div class="footer">
  <p>Currently learning by doing — homelab today, professional security work tomorrow.</p>
</div>

<!-- TYPING ANIMATION -->
<script>
(function() {
  const output = document.getElementById('term-output');
  const cursor = document.getElementById('term-cursor');
  if (!output) return;

  const commands = [
    {
      prompt: '$ ',
      text: 'whoami',
      result: 'cybersecurity student @ USF | homelab operator | AI tinkerer'
    },
    {
      prompt: '$ ',
      text: 'nmap -sV homelab.local',
      result: 'PORT      STATE  SERVICE\n443/tcp   open   nginx/1.24\n8080/tcp  open   python-flask\n3000/tcp  open   node.js\n5000/tcp  open   vLLM (CUDA 12.4)'
    },
    {
      prompt: '$ ',
      text: 'python3 exploit.py',
      result: '[+] Target: 192.168.1.10\n[+] Found: CVE-2024-1337\n[+] Exploit delivered\n[+] Shell received!'
    },
    {
      prompt: '$ ',
      text: 'nc -lvnp 4444',
      result: 'Connection from 10.0.0.5:48231\n# id\nuid=0(root) gid=0(root) euid=0(root)'
    },
    {
      prompt: '$ ',
      text: 'cat /root/flag.txt',
      result: '🏁 FLAG: HERMES{g00d_job_cyber_kid}'
    }
  ];

  let cmdIdx = 0;
  let charIdx = 0;
  let state = 'typing'; // typing | waiting | done

  function render() {
    let html = '';

    // Completed commands
    for (let i = 0; i < cmdIdx; i++) {
      html += `<span style="color:#6e7681;">${commands[i].prompt}${commands[i].text}</span>\n`;
      html += `<span style="color:#8b949e;">${commands[i].result.replace(/\n/g, '\n')}</span>\n\n`;
    }

    // Current command
    const cmd = commands[cmdIdx];
    if (state === 'typing') {
      html += `<span style="color:#6e7681;">${cmd.prompt}</span>`;
      html += `<span style="color:#7ee787;">${cmd.text.slice(0, charIdx)}</span>`;
      output.innerHTML = html;
      if (cursor) cursor.style.display = 'inline';
      charIdx++;
      if (charIdx > cmd.text.length + 1) {
        // Show full command + result
        html = '';
        for (let i = 0; i < cmdIdx; i++) {
          html += `<span style="color:#6e7681;">${commands[i].prompt}${commands[i].text}</span>\n`;
          html += `<span style="color:#8b949e;">${commands[i].result.replace(/\n/g, '\n')}</span>\n\n`;
        }
        html += `<span style="color:#6e7681;">${cmd.prompt}${cmd.text}</span>\n`;
        html += `<span style="color:#8b949e;">${cmd.result.replace(/\n/g, '\n')}</span>\n`;
        output.innerHTML = html;
        state = 'waiting';
        setTimeout(render, 2500);
        return;
      }
      setTimeout(render, 90);
    }
  }

  function advance() {
    cmdIdx++;
    if (cmdIdx >= commands.length) {
      setTimeout(function() {
        cmdIdx = 0;
        charIdx = 0;
        state = 'typing';
        render();
      }, 3000);
      return;
    }
    charIdx = 0;
    state = 'typing';
    render();
  }

  // Override for wait state
  const origRender = render;
  render = function() {
    if (state === 'typing') {
      let html = '';
      for (let i = 0; i < cmdIdx; i++) {
        html += `<span style="color:#6e7681;">${commands[i].prompt}${commands[i].text}</span>\n`;
        html += `<span style="color:#8b949e;">${commands[i].result.replace(/\n/g, '\n')}</span>\n\n`;
      }
      const cmd = commands[cmdIdx];
      html += `<span style="color:#6e7681;">${cmd.prompt}</span>`;
      html += `<span style="color:#7ee787;">${cmd.text.slice(0, charIdx)}</span>`;
      output.innerHTML = html;
      if (cursor) cursor.style.display = 'inline';
      charIdx++;
      if (charIdx > cmd.text.length + 1) {
        // Render complete command + result
        html = '';
        for (let i = 0; i < cmdIdx; i++) {
          html += `<span style="color:#6e7681;">${commands[i].prompt}${commands[i].text}</span>\n`;
          html += `<span style="color:#8b949e;">${commands[i].result.replace(/\n/g, '\n')}</span>\n\n`;
        }
        html += `<span style="color:#6e7681;">${cmd.prompt}${cmd.text}</span>\n`;
        html += `<span style="color:#8b949e;">${cmd.result.replace(/\n/g, '\n')}</span>\n`;
        output.innerHTML = html;
        state = 'waiting';
        setTimeout(render, 2500);
        return;
      }
      setTimeout(render, 90);
    } else if (state === 'waiting') {
      setTimeout(advance, 2500);
    }
  };

  render();
})();
</script>
</body>
</html>
