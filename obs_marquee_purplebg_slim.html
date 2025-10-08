<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>OBS 跑馬燈（半透明粉紫底・窄版）</title>
<style>
  :root{
    --height: 50px;  /* ✅ 調窄上下高度 */
    --font-size: 26px;
    --gap: 100px;
    --pps: 80;
    --text: #000;
    --shadow: none;
    --bg: rgba(230,200,255,0.6); /* 半透明粉紫底 */
    --padding-x: 18px;
    --weight: 700;
    --letter: 0.5px;
  }

  html, body { margin:0; padding:0; background:transparent; overflow:hidden; }

  .wrap{
    position:relative; width:100vw; height:var(--height);
    display:flex; align-items:center; padding:0 var(--padding-x);
    background:var(--bg); box-sizing:border-box;
    border-radius: 8px;
  }
  .viewport{ position:relative; width:100%; height:100%; overflow:hidden; }

  .track{
    position:absolute; top:50%; transform:translate3d(0,-50%,0);
    display:flex; flex-wrap:nowrap; white-space:nowrap; align-items:center;
    will-change:transform; backface-visibility:hidden; contain:content;
  }

  .segment{ display:inline-flex; align-items:center; gap:var(--gap); white-space:nowrap; }

  .item{
    display:inline-flex; align-items:center; gap:10px;
    white-space:nowrap;
    font-family: system-ui,-apple-system,"PingFang TC","Noto Sans TC","Microsoft JhengHei",Arial,sans-serif;
    font-size:var(--font-size); font-weight:var(--weight); letter-spacing:var(--letter);
    color:var(--text); text-shadow:var(--shadow);
    -webkit-font-smoothing: antialiased; text-rendering:optimizeLegibility;
  }
  .highlight{ color:#00b900; }
  .spacer{ width:var(--gap); height:1px; display:inline-block; }
</style>
</head>
<body>
  <div class="wrap">
    <div class="viewport">
      <div class="track" id="track"></div>
    </div>
  </div>

<script>
const messages = [
  '📱 LINE客服 : <span class="highlight">@225crrmi</span>',
  '⚠️ 請準時結單，避免影響下單權限',
  '🎁 直播不定時放福利，記得關注留言區'
];

const track = document.getElementById('track');

function buildSegment(){
  const seg = document.createElement('div');
  seg.className = 'segment';
  for(const m of messages){
    const d = document.createElement('div');
    d.className = 'item';
    d.innerHTML = m;
    seg.appendChild(d);
  }
  const spacer = document.createElement('span');
  spacer.className = 'spacer';
  seg.appendChild(spacer);
  return seg;
}

let segWidth = 0;
function layout(){
  track.innerHTML = '';
  const seg1 = buildSegment();
  track.appendChild(seg1);
  segWidth = seg1.getBoundingClientRect().width;
  const seg2 = seg1.cloneNode(true);
  track.appendChild(seg2);
  x = 0;
  track.style.transform = 'translate3d(0,-50%,0)';
}

let x = 0, last = performance.now();
function tick(t){
  const dt = (t - last) / 1000;
  last = t;
  const pps = parseFloat(getComputedStyle(document.documentElement).getPropertyValue('--pps')) || 80;
  x -= pps * dt;
  if (x <= -segWidth) x += segWidth;
  const xi = Math.floor(x);
  track.style.transform = `translate3d(${xi}px,-50%,0)`;
  requestAnimationFrame(tick);
}

window.addEventListener('load', ()=>{ layout(); last = performance.now(); requestAnimationFrame(tick); });
window.addEventListener('resize', ()=>{ layout(); });
</script>
</body>
</html>
