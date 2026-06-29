<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>毕业季的双重焦虑 · 数据新闻</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@300;400;500;700;900&display=swap');
*{margin:0;padding:0;box-sizing:border-box;}
:root{
  --pk:#C94F7C;--pkm:#E8729A;--pkl:#F5B8D0;--pkp:#FDE8F0;
  --pu:#8B5C9E;--pul:#C5A8D8;--pup:#F0E8F5;
  --tl:#5BBCB8;--bl:#7BB8D4;--or:#F0894A;
  --cr:#FFF8FB;--gr:#6B6B6B;--dk:#2D1A26;
}
body{font-family:'Noto Sans SC','PingFang SC','Microsoft YaHei',sans-serif;background:var(--cr);color:var(--dk);max-width:480px;margin:0 auto;overflow-x:hidden;}

/* HERO */
.hero{background:linear-gradient(160deg,#C94F7C 0%,#8B5C9E 55%,#4A2070 100%);padding:52px 28px 62px;position:relative;overflow:hidden;text-align:center;}
.hero::before{content:'';position:absolute;top:-80px;right:-80px;width:260px;height:260px;border-radius:50%;background:rgba(255,255,255,0.05);}
.hero::after{content:'';position:absolute;bottom:-60px;left:-60px;width:200px;height:200px;border-radius:50%;background:rgba(255,255,255,0.04);}
.hero-tag{display:inline-block;background:rgba(255,255,255,0.18);color:#fff;font-size:11px;letter-spacing:2px;padding:5px 16px;border-radius:20px;margin-bottom:22px;}
.hero h1{color:#fff;font-size:28px;font-weight:900;line-height:1.35;margin-bottom:14px;}
.hero h1 em{font-style:normal;color:#FFD6E8;}
.hero-lead{color:rgba(255,255,255,0.85);font-size:13.5px;line-height:1.9;margin-bottom:12px;}
.hero-meta{color:rgba(255,255,255,0.5);font-size:11px;margin-bottom:36px;}
.hero-stats{display:flex;border-top:1px solid rgba(255,255,255,0.2);padding-top:28px;}
.hstat{flex:1;text-align:center;border-right:1px solid rgba(255,255,255,0.15);padding:0 6px;}
.hstat:last-child{border-right:none;}
.hnum{font-size:34px;font-weight:900;color:#FFD6E8;line-height:1;}
.hnum sup{font-size:16px;}
.hlbl{font-size:10px;color:rgba(255,255,255,0.65);margin-top:5px;line-height:1.5;}

/* INTRO */
.intro{background:linear-gradient(135deg,#F5B8D0,#C5A8D8);padding:24px 26px;}
.intro p{font-size:13.5px;line-height:1.95;color:#2D1A26;}
.intro strong{color:var(--pk);}

/* SECTION */
.sec{padding:40px 24px 36px;}
.s-w{background:#fff;}
.s-pk{background:var(--pkp);}
.s-pu{background:var(--pup);}
.s-dk{background:linear-gradient(135deg,#2D1A26,#4A1F3F);color:#fff;}
.s-tl{background:#F0FAFA;}
.s-or{background:#FFF6F0;}

.badge{display:inline-flex;align-items:center;justify-content:center;width:30px;height:30px;border-radius:50%;background:var(--pk);color:#fff;font-size:12px;font-weight:700;margin-bottom:12px;}
.badge-lt{background:rgba(255,255,255,0.2);}
.eyebrow{font-size:10px;letter-spacing:2.5px;font-weight:700;color:var(--pk);margin-bottom:6px;}
.eyebrow-lt{color:var(--pkl);}
.eyebrow-pu{color:var(--pu);}
.eyebrow-tl{color:var(--tl);}
.eyebrow-or{color:var(--or);}
.stitle{font-size:22px;font-weight:900;line-height:1.38;margin-bottom:14px;}
.stitle-lt{color:#fff;}
.body{font-size:13.5px;line-height:1.95;color:var(--gr);}
.body-lt{color:rgba(255,255,255,0.78);}
.body strong{color:var(--pk);}
.body-lt strong{color:#FFD6E8;}

/* QUOTE */
.qb{background:linear-gradient(135deg,var(--pkp),var(--pup));border-left:4px solid var(--pk);border-radius:0 14px 14px 0;padding:18px 20px;margin:20px 0;font-size:13px;color:var(--dk);line-height:1.85;font-style:italic;}
.qb cite{display:block;font-style:normal;font-size:11.5px;color:var(--pk);font-weight:600;margin-top:10px;}

/* CALLOUT */
.callout{border-radius:14px;padding:18px 20px;margin:20px 0;display:flex;align-items:center;gap:16px;}
.callout.pk{background:var(--pk);}
.callout.pu{background:var(--pu);}
.callout.soft{background:linear-gradient(135deg,var(--pkm),var(--pu));}
.callout.tl{background:var(--tl);}
.cnum{font-size:46px;font-weight:900;color:#fff;line-height:1;flex-shrink:0;}
.cnum sup{font-size:22px;}
.clbl{font-size:13px;color:rgba(255,255,255,0.92);line-height:1.7;}

/* STAT GRID */
.sgrid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin:20px 0;}
.sc{background:#fff;border-radius:14px;padding:16px 12px;text-align:center;box-shadow:0 3px 16px rgba(201,79,124,0.1);}
.sc.pk{background:linear-gradient(135deg,#C94F7C,#8B5C9E);}
.sc.pu{background:linear-gradient(135deg,#8B5C9E,#5B3A7E);}
.sc.tl{background:linear-gradient(135deg,#5BBCB8,#2E8B88);}
.scn{font-size:32px;font-weight:900;color:var(--pk);line-height:1;}
.scn.w{color:#fff;}
.scn sup{font-size:14px;}
.scl{font-size:11.5px;color:var(--gr);margin-top:6px;line-height:1.55;}
.scl.w{color:rgba(255,255,255,0.85);}

/* DIVIDER */
.div{height:2px;background:linear-gradient(90deg,var(--pkl),transparent);margin:26px 0;}
.div-lt{background:linear-gradient(90deg,rgba(255,255,255,0.25),transparent);}

/* CHART LABELS */
.chart-title{font-size:12px;color:var(--gr);font-weight:600;margin-bottom:14px;}

/* ── CHART 1: HORIZONTAL BAR ── */
.hbar-wrap{margin:20px 0;}
.hbar-item{margin-bottom:18px;}
.hbar-meta{display:flex;justify-content:space-between;align-items:baseline;margin-bottom:5px;}
.hbar-name{font-size:12.5px;color:var(--dk);font-weight:500;flex:1;padding-right:8px;}
.hbar-pct{font-size:15px;font-weight:700;color:var(--pk);flex-shrink:0;}
.hbar-pct.pu{color:var(--pu);}
.hbar-pct.tl{color:var(--tl);}
.hbar-sub{font-size:11px;color:var(--gr);margin-bottom:5px;line-height:1.5;}
.track{background:#EDD5E5;border-radius:20px;height:11px;overflow:hidden;}
.track.pu{background:#DDD0EA;}
.track.tl{background:#C8EDED;}
.track.dk{background:rgba(255,255,255,0.1);}
.fill{height:100%;border-radius:20px;width:0;transition:width 1.3s cubic-bezier(.4,0,.2,1);}
.f-pk{background:linear-gradient(90deg,#C94F7C,#8B5C9E);}
.f-pu{background:linear-gradient(90deg,#8B5C9E,#5B3A7E);}
.f-tl{background:linear-gradient(90deg,#5BBCB8,#2E8B88);}
.f-bl{background:linear-gradient(90deg,#7BB8D4,#4A99BF);}
.f-or{background:linear-gradient(90deg,#F0894A,#D4601A);}
.f-hot{background:linear-gradient(90deg,#FF3D6B,#CC1A50);}
.f-soft{background:linear-gradient(90deg,#E8729A,#C5A8D8);}
.f-lt{background:linear-gradient(90deg,rgba(245,184,208,0.8),rgba(197,168,216,0.8));}

/* ── CHART 2: DONUT / PIE SVG ── */
.donut-row{display:flex;align-items:center;gap:18px;margin:20px 0;}
.donut-row svg{flex-shrink:0;}
.dleg{flex:1;}
.drow{display:flex;align-items:flex-start;gap:8px;margin-bottom:11px;}
.ddot{width:10px;height:10px;border-radius:50%;flex-shrink:0;margin-top:3px;}
.dtxt{font-size:12px;color:var(--dk);flex:1;line-height:1.5;}
.dpct{font-size:14px;font-weight:700;flex-shrink:0;}

/* ── CHART 3: BUBBLE CHART (CSS) ── */
.bubble-wrap{margin:20px 0;position:relative;height:220px;}
.bubble{position:absolute;border-radius:50%;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;}
.b-num{font-size:18px;font-weight:900;color:#fff;line-height:1;}
.b-lbl{font-size:10px;color:rgba(255,255,255,0.9);margin-top:3px;line-height:1.3;padding:0 4px;}

/* ── CHART 4: STEP / TIMELINE ── */
.timeline{margin:20px 0;position:relative;padding-left:28px;}
.timeline::before{content:'';position:absolute;left:10px;top:0;bottom:0;width:2px;background:linear-gradient(180deg,var(--pk),var(--pu));}
.tl-item{position:relative;margin-bottom:24px;}
.tl-item::before{content:'';position:absolute;left:-24px;top:6px;width:12px;height:12px;border-radius:50%;background:var(--pk);border:2px solid #fff;box-shadow:0 0 0 2px var(--pk);}
.tl-pct{font-size:26px;font-weight:900;color:var(--pk);line-height:1.1;}
.tl-title{font-size:13.5px;font-weight:700;color:var(--dk);margin:3px 0;}
.tl-desc{font-size:12px;color:var(--gr);line-height:1.7;}

/* ── CHART 5: STACKED BAR ── */
.sbar-wrap{margin:20px 0;}
.sbar-row{margin-bottom:16px;}
.sbar-label{font-size:12px;color:var(--dk);font-weight:500;margin-bottom:5px;}
.sbar-track{display:flex;height:26px;border-radius:13px;overflow:hidden;}
.seg{height:100%;display:flex;align-items:center;justify-content:center;font-size:10px;color:#fff;font-weight:600;transition:width 1.3s cubic-bezier(.4,0,.2,1);width:0;}

/* ── CHART 6: LOLLIPOP ── */
.lollipop-wrap{margin:20px 0;}
.lp-item{display:flex;align-items:center;gap:10px;margin-bottom:16px;}
.lp-name{font-size:12px;color:var(--dk);width:80px;flex-shrink:0;text-align:right;font-weight:500;}
.lp-line-wrap{flex:1;position:relative;height:14px;display:flex;align-items:center;}
.lp-line{height:3px;border-radius:3px;width:0;transition:width 1.3s cubic-bezier(.4,0,.2,1);}
.lp-dot{width:14px;height:14px;border-radius:50%;position:absolute;right:-1px;top:50%;transform:translateY(-50%);border:2px solid #fff;box-shadow:0 2px 6px rgba(0,0,0,0.15);}
.lp-pct{font-size:13px;font-weight:700;color:var(--pk);width:48px;flex-shrink:0;}

/* ── CHART 7: RADAR (SVG) ── */
.radar-wrap{margin:20px 0;text-align:center;}
.radar-leg{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin-top:12px;}
.radar-leg-item{display:flex;align-items:center;gap:5px;font-size:11px;color:var(--gr);}
.radar-leg-dot{width:8px;height:8px;border-radius:50%;}

/* ── CHART 8: PRICE BAR (horizontal with icons) ── */
.price-wrap{margin:20px 0;}
.pr-row{background:#fff;border-radius:12px;padding:14px 16px;margin-bottom:8px;box-shadow:0 2px 10px rgba(201,79,124,0.08);}
.pr-top{display:flex;justify-content:space-between;align-items:center;margin-bottom:6px;}
.pr-name{font-size:13px;font-weight:600;color:var(--dk);}
.pr-amt{font-size:20px;font-weight:900;color:var(--pk);}
.pr-amt small{font-size:11px;font-weight:400;color:var(--gr);}
.pr-bar-track{background:#EDD5E5;border-radius:10px;height:7px;overflow:hidden;}
.pr-bar-fill{height:100%;border-radius:10px;background:linear-gradient(90deg,var(--pk),var(--pu));width:0;transition:width 1.3s cubic-bezier(.4,0,.2,1);}

/* ── ANNOTATION BOX ── */
.anno{background:rgba(201,79,124,0.08);border:1px dashed var(--pkl);border-radius:12px;padding:14px 16px;margin:14px 0;}
.anno p{font-size:12.5px;color:var(--dk);line-height:1.8;}
.anno strong{color:var(--pk);}

/* tags */
.tag-row{display:flex;flex-wrap:wrap;gap:8px;margin:16px 0;}
.tag{padding:6px 14px;border-radius:20px;font-size:12px;font-weight:500;}
.t-pk{background:var(--pkp);color:var(--pk);border:1px solid var(--pkl);}
.t-pu{background:var(--pup);color:var(--pu);border:1px solid var(--pul);}
.t-tl{background:#E8F8F8;color:var(--tl);border:1px solid #A8DFDD;}

/* CONCLUSION */
.conclusion{background:linear-gradient(160deg,#C94F7C,#8B5C9E,#4A2070);padding:56px 28px 70px;text-align:center;color:#fff;}
.con-icon{font-size:46px;display:block;margin-bottom:16px;}
.con-title{font-size:25px;font-weight:900;line-height:1.4;margin-bottom:20px;}
.con-body{font-size:13.5px;color:rgba(255,255,255,0.82);line-height:1.95;margin-bottom:30px;}
.con-pill{display:inline-block;background:rgba(255,255,255,0.15);border:1px solid rgba(255,255,255,0.3);border-radius:30px;padding:8px 22px;font-size:13px;color:#fff;margin:4px;}

/* FOOTER */
.footer{background:var(--dk);color:rgba(255,255,255,0.42);font-size:11px;text-align:center;padding:24px 24px;line-height:2;}

/* WAVE */
.wave{display:block;width:100%;overflow:hidden;line-height:0;}
mark{background:linear-gradient(180deg,transparent 55%,#F5B8D0 55%);color:inherit;padding:0 2px;}
</style>
</head>
<body>

<!-- ══ HERO ══ -->
<section class="hero">
  <div class="hero-tag">📊 数据新闻 · 2026毕业季</div>
  <h1>毕业季的<em>双重焦虑</em><br>查重+AI 双检时代<br>大学生的论文生存图鉴</h1>
  <p class="hero-lead">当97%的学生都在用AI写论文，高校却用一套并不成熟的技术画出15%–40%的红线。一边是检测技术的"黑箱"误判，一边是动辄几百元的检测费用，再加上无法毕业的恐惧——2026年的毕业季，大学生们正在经历一场前所未有的双重焦虑。</p>
  <p class="hero-meta">中国海洋大学 · 2023级网络与新媒体 · 第六小组 · 有效样本 N=217</p>
  <div class="hero-stats">
    <div class="hstat"><div class="hnum">97<sup>%</sup></div><div class="hlbl">论文写作<br>中使用AI</div></div>
    <div class="hstat"><div class="hnum">42<sup>%</sup></div><div class="hlbl">高校全面<br>双重检测</div></div>
    <div class="hstat"><div class="hnum">70<sup>%</sup></div><div class="hlbl">担心无法<br>顺利毕业</div></div>
    <div class="hstat"><div class="hnum">62<sup>%</sup></div><div class="hlbl">认为AI检<br>测存误判</div></div>
  </div>
</section>

<!-- INTRO -->
<div class="intro">
  <p>朱自清的《荷塘月色》上传至AI检测系统，竟被判定AI生成内容超过<strong>60%</strong>；一位手搓论文的学生一字一字敲出来，AI率高达<strong>80%</strong>。这不是段子，而是如今高校毕业生正在面对的现实。四川大学、南京工业大学、广西师范大学、河北工程大学等高校相继发布通知，要求本科毕业论文须进行AIGC检测。一边是<strong>97%的学生在用AI</strong>，一边是高校用并不成熟的检测技术设置<strong>15%–40%</strong>的红线，标准五花八门，但共同点只有一个：超过规定上限，论文不得参加盲审和答辩。</p>
</div>

<svg class="wave" viewBox="0 0 480 24" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg"><path d="M0,0 C120,24 360,0 480,16 L480,24 L0,24Z" fill="#fff"/></svg>

<!-- ══ S1: 双重检测现状 · 分组横向条形图 ══ -->
<section class="sec s-w">
  <div class="badge">01</div>
  <p class="eyebrow">检测制度现状</p>
  <h2 class="stitle">"双重检测"已成常态<br>41.94% 高校全面铺开</h2>
  <p class="body">根据《大学生毕业论文查重调查问卷》有效样本217份的数据，<strong>41.94%</strong>的高校已全面实行"查重+AI双重检测"，仅开展AI检测无传统查重的占25.35%，仅开展传统查重无AI检测的占24.88%，暂未开展任何检测的仅占7.83%。换句话说，<strong>超过九成高校已开展某种形式的论文检测</strong>，超过67%的高校已将AI检测纳入审核体系——这已不是个别现象，而是一场席卷全国的制度变革。</p>

  <!-- 图表1：水平分组条形图 -->
  <div class="hbar-wrap" style="margin-top:24px;">
    <p class="chart-title">▌ 国内高校论文检测模式分布（N=217）</p>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">全面实行查重+AI双重检测</span><span class="hbar-pct">41.94%</span></div>
      <div class="hbar-sub">超过四成高校同时启用传统查重与AIGC内容检测</div>
      <div class="track"><div class="fill f-pk" data-w="41.94"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">仅开展AI检测（无传统查重）</span><span class="hbar-pct">25.35%</span></div>
      <div class="hbar-sub">部分高校新引入AI检测，暂未同步推广传统查重</div>
      <div class="track"><div class="fill f-soft" data-w="25.35"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">仅开展传统查重（无AI检测）</span><span class="hbar-pct">24.88%</span></div>
      <div class="hbar-sub">仍沿用知网/维普等传统查重体系，尚未引入AI检测</div>
      <div class="track"><div class="fill f-bl" data-w="24.88"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">暂未开展任何检测</span><span class="hbar-pct">7.83%</span></div>
      <div class="hbar-sub">极少数学校目前尚未要求论文检测</div>
      <div class="track"><div class="fill f-lt" data-w="7.83"></div></div>
    </div>
  </div>

  <div class="div"></div>

  <!-- 图表2：各校AI率标准气泡图(CSS) -->
  <p class="chart-title">▌ 各高校AI生成内容容忍上限对比</p>
  <div class="bubble-wrap">
    <div class="bubble" style="width:110px;height:110px;background:linear-gradient(135deg,#C94F7C,#8B5C9E);left:10px;top:10px;">
      <span class="b-num">≤15%</span>
      <span class="b-lbl">四川大学<br>理工医科</span>
    </div>
    <div class="bubble" style="width:90px;height:90px;background:linear-gradient(135deg,#8B5C9E,#5B3A7E);left:130px;top:0px;">
      <span class="b-num">≤20%</span>
      <span class="b-lbl">四川大学<br>文科</span>
    </div>
    <div class="bubble" style="width:100px;height:100px;background:linear-gradient(135deg,#5BBCB8,#2E8B88);left:232px;top:8px;">
      <span class="b-num">≤25%</span>
      <span class="b-lbl">上交大<br>浙大</span>
    </div>
    <div class="bubble" style="width:88px;height:88px;background:linear-gradient(135deg,#7BB8D4,#4A80A0);left:22px;top:118px;">
      <span class="b-num">≤30%</span>
      <span class="b-lbl">复旦 南大<br>海大</span>
    </div>
    <div class="bubble" style="width:80px;height:80px;background:linear-gradient(135deg,#F0894A,#C96030);left:128px;top:108px;">
      <span class="b-num">≤35%</span>
      <span class="b-lbl">华中<br>理工</span>
    </div>
    <div class="bubble" style="width:96px;height:96px;background:linear-gradient(135deg,#E84393,#9B1C5E);left:222px;top:118px;">
      <span class="b-num">≤40%</span>
      <span class="b-lbl">南航<br>天大</span>
    </div>
  </div>
  <p style="font-size:11px;color:var(--gr);text-align:center;margin-top:4px;">气泡大小反映相对宽松程度 · 数据来源：各高校教务处公开文件及2026年媒体汇总</p>

  <p class="body" style="margin-top:18px;">各校对AI生成内容的容忍度差异巨大，检测标准大致分为五档，此外还有部分院系实行自主标准。<strong>标准差距最大达25个百分点</strong>，同一篇论文在不同高校可能呈现截然不同的审核结果——这种标准不统一本身，已构成制度层面的公平性隐患。</p>

  <div class="qb">北京工商大学明确规定了2026届本科毕业生使用AI工具的"三原则"：<strong>"学术诚信为本、合理辅助为限、责任自负原则"</strong>，不得将AI直接生成内容作为论文核心观点或数据分析结论，所有AI生成内容需在脚注中标注使用场景和工具名称——这或许是目前最具操作性的规范探索之一。<cite>——各高校教务处公开毕业文件</cite></div>
</section>

<svg class="wave" viewBox="0 0 480 24" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg"><path d="M0,24 C120,0 360,24 480,8 L480,0 L0,0Z" fill="#fff"/><path d="M0,24 C120,0 360,24 480,8 L480,24 L0,24Z" fill="var(--pkp)"/></svg>

<!-- ══ S2: AI误判困境 · 饼图+堆叠 ══ -->
<section class="sec s-pk">
  <div class="badge">02</div>
  <p class="eyebrow">技术争议</p>
  <h2 class="stitle">AI检测的"误伤"困境：<br>原创与AI的模糊边界</h2>
  <p class="body">AI检测技术本身存在巨大争议。收费标准高、检测过程过于"黑箱"、检测结果不稳定……许多大学生和高校教师质疑，当前高校检测AIGC率的手段并不科学。更离谱的是，<strong>逻辑严谨、用词规范的原创内容被频频误判</strong>，原因正在于AI写作本身倾向于规范流畅的表达。有学生反映，自己认为流畅通顺的句子全被判为AI生成；上下两段语言风格和逻辑完全相同，只有其中一段被标红；不同检测平台的结果差异甚至超过<strong>20个百分点</strong>。</p>

  <div class="callout pk" style="margin-top:20px;">
    <div class="cnum">62<sup>%</sup></div>
    <div class="clbl">超过六成学生认为AI检测存在不同程度的误判问题，其中35.48%认为"<strong>普遍存在误判，原创也会被标记</strong>"——这是所有选项中占比最高的单项。</div>
  </div>

  <!-- 图表3：SVG饼图 -->
  <p class="chart-title" style="margin-top:6px;">▌ 学生对AI检测误判的认知分布（N=217）</p>
  <div class="donut-row">
    <svg width="130" height="130" viewBox="0 0 42 42">
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#EDD5E5" stroke-width="9"/>
      <!-- 35.48% hot pink -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#C94F7C" stroke-width="9"
        stroke-dasharray="35.48 64.52" stroke-dashoffset="25"/>
      <!-- 26.73% purple -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#8B5C9E" stroke-width="9"
        stroke-dasharray="26.73 73.27" stroke-dashoffset="-10.48"/>
      <!-- 33.18% teal -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#5BBCB8" stroke-width="9"
        stroke-dasharray="33.18 66.82" stroke-dashoffset="-37.21"/>
      <!-- 4.61% gray -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#C5A8D8" stroke-width="9"
        stroke-dasharray="4.61 95.39" stroke-dashoffset="-70.39"/>
      <text x="21" y="19.5" text-anchor="middle" font-size="4.5" font-weight="bold" fill="#C94F7C">超六成</text>
      <text x="21" y="24" text-anchor="middle" font-size="3.5" fill="#6B6B6B">认为有误判</text>
    </svg>
    <div class="dleg">
      <div class="drow"><div class="ddot" style="background:#C94F7C"></div><span class="dtxt">普遍存在误判，原创也被标记</span><span class="dpct" style="color:#C94F7C">35.48%</span></div>
      <div class="drow"><div class="ddot" style="background:#8B5C9E"></div><span class="dtxt">偶尔出现误判</span><span class="dpct" style="color:#8B5C9E">26.73%</span></div>
      <div class="drow"><div class="ddot" style="background:#5BBCB8"></div><span class="dtxt">判定基本准确，无误判</span><span class="dpct" style="color:#5BBCB8">33.18%</span></div>
      <div class="drow"><div class="ddot" style="background:#C5A8D8"></div><span class="dtxt">不了解检测逻辑</span><span class="dpct" style="color:#9B8AAA">4.61%</span></div>
    </div>
  </div>

  <div class="qb">
    "自己认为流畅通顺的句子全被判为AI生成，更令人费解的是，上下两段语言风格和逻辑完全相同，只有其中一段被标红。"
    <cite>——受访大学生留言（《大学生毕业论文查重调查问卷》）</cite>
  </div>

  <p class="body">当检测工具本身都不够可靠时，用它来判定一个学生能否毕业，<strong>公平吗？</strong>这个问题没有标准答案，但62%的学生用亲身经历给出了自己的判断。在高校用"检测结果"直接关联毕业资格的制度设计下，这种不确定性正在演变成一种系统性的不公平。</p>

  <!-- 图表4：堆叠条形图（焦虑维度） -->
  <div class="div" style="margin-top:24px;"></div>
  <p class="chart-title">▌ 学生因双检产生的多重焦虑程度（完全符合→完全不符合）</p>
  <div class="sbar-wrap">
    <div class="sbar-row">
      <div class="sbar-label">同时面对双检感到焦虑不安</div>
      <div class="sbar-track">
        <div class="seg" style="background:#C94F7C;" data-w="38">38%</div>
        <div class="seg" style="background:#E8729A;" data-w="32">32%</div>
        <div class="seg" style="background:#C5A8D8;" data-w="20">20%</div>
        <div class="seg" style="background:#EDD5E5;" data-w="10">10%</div>
      </div>
    </div>
    <div class="sbar-row">
      <div class="sbar-label">担心论文无法按时通过检测</div>
      <div class="sbar-track">
        <div class="seg" style="background:#8B5C9E;" data-w="41">41%</div>
        <div class="seg" style="background:#C5A8D8;" data-w="29">29%</div>
        <div class="seg" style="background:#DDD0EA;" data-w="19">19%</div>
        <div class="seg" style="background:#F0E8F5;" data-w="11">11%</div>
      </div>
    </div>
    <div class="sbar-row">
      <div class="sbar-label">标准严苛限制写作自由</div>
      <div class="sbar-track">
        <div class="seg" style="background:#C94F7C;" data-w="35">35%</div>
        <div class="seg" style="background:#E8729A;" data-w="28">28%</div>
        <div class="seg" style="background:#C5A8D8;" data-w="22">22%</div>
        <div class="seg" style="background:#EDD5E5;" data-w="15">15%</div>
      </div>
    </div>
    <div class="sbar-row">
      <div class="sbar-label">担忧误判不敢使用AI</div>
      <div class="sbar-track">
        <div class="seg" style="background:#5BBCB8;" data-w="30">30%</div>
        <div class="seg" style="background:#90D0CD;" data-w="33">33%</div>
        <div class="seg" style="background:#C8EDED;" data-w="24">24%</div>
        <div class="seg" style="background:#E8F8F8;" data-w="13">13%</div>
      </div>
    </div>
  </div>
  <div style="display:flex;gap:6px;flex-wrap:wrap;margin-top:8px;">
    <span style="display:flex;align-items:center;gap:4px;font-size:10.5px;color:var(--gr);"><span style="width:10px;height:10px;border-radius:2px;background:#C94F7C;display:inline-block;"></span>完全符合</span>
    <span style="display:flex;align-items:center;gap:4px;font-size:10.5px;color:var(--gr);"><span style="width:10px;height:10px;border-radius:2px;background:#E8729A;display:inline-block;"></span>比较符合</span>
    <span style="display:flex;align-items:center;gap:4px;font-size:10.5px;color:var(--gr);"><span style="width:10px;height:10px;border-radius:2px;background:#C5A8D8;display:inline-block;"></span>一般</span>
    <span style="display:flex;align-items:center;gap:4px;font-size:10.5px;color:var(--gr);"><span style="width:10px;height:10px;border-radius:2px;background:#EDD5E5;display:inline-block;"></span>完全不符合</span>
  </div>
</section>

<svg class="wave" viewBox="0 0 480 24" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg"><path d="M0,0 C120,24 360,0 480,16 L480,24 L0,24Z" fill="var(--pup)"/></svg>

<!-- ══ S3: 学生使用AI场景 · 棒棒糖图 ══ -->
<section class="sec s-pu">
  <div class="badge" style="background:var(--pu)">03</div>
  <p class="eyebrow eyebrow-pu">学生AI使用现状</p>
  <h2 class="stitle">97% 的学生都在用AI<br>近半数用它来规避检测</h2>
  <p class="body">前文提到的大学生AI使用场景的调查数据揭示了令人深思的矛盾：AI工具使用率极高，从语句润色、文献检索，到框架搭建、段落生成，AI几乎渗透了论文写作的每一个环节。而<strong>最值得关注的是：45.37%的学生使用AI的目的之一，是"改写文本、规避AI检测"</strong>——也就是说，近半数使用AI的学生，是为了让论文"看起来不像AI写的"。这个数字本身，已经宣告了"用AI检测来防止学生用AI"这一逻辑的内在矛盾。</p>

  <!-- 图表5：棒棒糖图 -->
  <div class="lollipop-wrap" style="margin-top:24px;">
    <p class="chart-title">▌ 大学生AI工具使用场景占比排行（N=217）</p>
    <div class="lp-item">
      <span class="lp-name" style="font-size:11px;">语句润色<br>优化表达</span>
      <div class="lp-line-wrap">
        <div class="lp-line f-pk" data-w="97.07" style="background:linear-gradient(90deg,#C94F7C,#8B5C9E);"></div>
        <div class="lp-dot" style="background:#C94F7C;right:calc(0%);"></div>
      </div>
      <span class="lp-pct">97.07%</span>
    </div>
    <div class="lp-item">
      <span class="lp-name" style="font-size:11px;">文献检索<br>外文翻译</span>
      <div class="lp-line-wrap">
        <div class="lp-line f-pk" data-w="85.85" style="background:linear-gradient(90deg,#C94F7C,#8B5C9E);"></div>
        <div class="lp-dot" style="background:#8B5C9E;right:calc(0%);"></div>
      </div>
      <span class="lp-pct">85.85%</span>
    </div>
    <div class="lp-item">
      <span class="lp-name" style="font-size:11px;">搭建框架<br>梳理思路</span>
      <div class="lp-line-wrap">
        <div class="lp-line f-pk" data-w="78.05" style="background:linear-gradient(90deg,#C94F7C,#8B5C9E);"></div>
        <div class="lp-dot" style="background:#5B3A7E;right:calc(0%);"></div>
      </div>
      <span class="lp-pct">78.05%</span>
    </div>
    <div class="lp-item">
      <span class="lp-name" style="font-size:11px;">直接生成<br>段落/全文</span>
      <div class="lp-line-wrap">
        <div class="lp-line f-bl" data-w="51.22" style="background:linear-gradient(90deg,#7BB8D4,#4A80A0);"></div>
        <div class="lp-dot" style="background:#7BB8D4;right:calc(0%);"></div>
      </div>
      <span class="lp-pct" style="color:#7BB8D4;">51.22%</span>
    </div>
    <div class="lp-item">
      <span class="lp-name" style="font-size:11px;color:var(--pk);font-weight:700;">⚠ 改写文本<br>规避AI检测</span>
      <div class="lp-line-wrap">
        <div class="lp-line f-hot" data-w="45.37" style="background:linear-gradient(90deg,#FF3D6B,#CC1A50);"></div>
        <div class="lp-dot" style="background:#FF3D6B;right:calc(0%);"></div>
      </div>
      <span class="lp-pct" style="color:#FF3D6B;">45.37%</span>
    </div>
  </div>

  <div class="callout soft">
    <div class="cnum" style="font-size:36px;">矛盾</div>
    <div class="clbl">高校用AI检测来防止学生"用AI"，学生却用AI来规避AI检测。这场博弈，形成了一个<strong>荒诞的闭环</strong>：检测越严，规避越精；规避越精，检测越难。</div>
  </div>
</section>

<svg class="wave" viewBox="0 0 480 24" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg"><path d="M0,24 C120,0 360,24 480,8 L480,0 L0,0Z" fill="var(--pup)"/><path d="M0,24 C120,0 360,24 480,8 L480,24 L0,24Z" fill="#fff"/></svg>

<!-- ══ S4: 博弈策略 · 时间轴 ══ -->
<section class="sec s-w">
  <div class="badge">04</div>
  <p class="eyebrow">学生应对策略</p>
  <h2 class="stitle">用AI对抗AI检测<br>已成普遍应对策略</h2>
  <p class="body">面对AI检测压力，学生使出了浑身解数。调查问卷显示，几乎所有使用过AI的学生都采取了某种形式的"应对措施"。这些策略从成本到效果各不相同，但有一个共同点：<strong>它们耗费了学生大量本可用于学术研究的时间和精力</strong>，让"写一篇好论文"这件本应是核心目标的事，反而被边缘化。</p>

  <!-- 图表6：时间轴/步骤图 -->
  <div class="timeline" style="margin-top:24px;">
    <p class="chart-title" style="margin-left:-28px;">▌ 学生应对AI检测的主要策略（N=217）</p>
    <div class="tl-item">
      <div class="tl-pct">92.17%</div>
      <div class="tl-title">更换多款AI交叉生成文本</div>
      <div class="tl-desc">用DeepSeek、ChatGPT、文心一言、Kimi等多个平台反复生成同一段落，再混合剪裁，以"稀释"单一AI写作特征，降低被标记概率。这是目前<strong>最主流的规避策略</strong>，但也意味着学生需要在多个平台之间来回切换，生成、比对、筛选，消耗大量时间。</div>
    </div>
    <div class="tl-item">
      <div class="tl-pct" style="color:var(--pu);">86.64%</div>
      <div class="tl-title">AI生成内容人工逐句改写</div>
      <div class="tl-desc">将AI输出的段落一句一句用自己的语言重新表达。这是被认为最"正当"的方式，但也是最耗时的——为了改写一篇1.5万字的论文，有学生耗费了<strong>超过40小时</strong>在逐字修改上。很多人宁愿花数倍时间改写，也不愿完全放弃使用AI。</div>
    </div>
    <div class="tl-item">
      <div class="tl-pct" style="color:var(--tl);">72.81%</div>
      <div class="tl-title">直接放弃使用所有AI工具</div>
      <div class="tl-desc">部分学生在了解检测机制后选择"断AI"，回归全手写。但这并不意味着他们认为禁AI合理，更多是一种无奈的妥协——因为被误判的代价太高，他们无法承受答辩被取消的风险。</div>
    </div>
    <div class="tl-item">
      <div class="tl-pct" style="color:var(--or);">58.53%</div>
      <div class="tl-title">专门学习避检技巧</div>
      <div class="tl-desc">在小红书、B站、学习社群中，"如何降低AIGC率"已成热门话题。有学生系统研究检测算法逻辑，总结出句式变换、标点替换、专业词汇插入、长短句交替等"避雷手册"，并在社群中广泛传播。<strong>反制技术生态已然形成。</strong></div>
    </div>
  </div>

  <div class="div"></div>
  <p class="chart-title">▌ 学生论文被AI检测标记的实际结果（N=217）</p>
  <div class="sgrid">
    <div class="sc pk"><div class="scn w">45.62<sup>%</sup></div><div class="scl w">判定1次<br>修改后合格</div></div>
    <div class="sc"><div class="scn" style="color:var(--or);font-size:28px;">近<span style="font-size:38px">3</span>成</div><div class="scl">多次判定<br>反复修改循环</div></div>
    <div class="sc"><div class="scn">17.97<sup>%</sup></div><div class="scl">未被判定<br>出AI内容</div></div>
    <div class="sc" style="background:var(--pkp);"><div class="scn" style="font-size:24px;">7.37<sup>%</sup></div><div class="scl">暂未参与<br>AI检测</div></div>
  </div>
  <p class="body" style="margin-top:12px;">近三成学生经历了多次判定、反复修改的循环。而"AI生成内容人工逐句改写"成为86.64%学生的选择——<strong>很多人宁愿花大量时间人工改写AI生成的内容，也不愿完全放弃使用AI</strong>，这本身说明AI工具对学生的写作效率提升已达到了难以割舍的程度。</p>
</section>

<!-- ══ S5: 焦虑与费用 · 价格条形+折线 ══ -->
<section class="sec s-dk">
  <div class="badge badge-lt">05</div>
  <p class="eyebrow eyebrow-lt">双检带来的后果</p>
  <h2 class="stitle stitle-lt">近七成学生担心<br>双检不通过，无法毕业</h2>
  <p class="body body-lt">当查重和AI检测双重压力叠加，焦虑成为毕业论文创作中的普遍情绪。这种焦虑不是抽象的——它具体地体现在<strong>查重次数的累积</strong>和<strong>真实金钱的支出</strong>上。调查数据显示，近六成学生查重次数在2次以上，近两成超过4次；而每次检测都需要自费，论文还没写完，检测费已花了数百元。</p>

  <div class="callout" style="background:rgba(255,255,255,0.12);border:1px solid rgba(255,255,255,0.2);margin-top:20px;">
    <div class="cnum" style="color:#FFD6E8;">近6成</div>
    <div class="clbl" style="color:rgba(255,255,255,0.9);">学生查重次数在<strong>2次以上</strong>，近两成超过<strong>4次</strong>。检测费用累积，论文未完成，支出已超百元。</div>
  </div>

  <!-- 图表7：查重次数水平条形图 -->
  <div class="hbar-wrap" style="margin-top:20px;">
    <p class="chart-title" style="color:rgba(255,255,255,0.55);">▌ 学生论文累计查重次数分布（N=217）</p>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name" style="color:rgba(255,255,255,0.85);">4次及以上</span><span class="hbar-pct" style="color:#FFD6E8;">18.89%</span></div>
      <div class="track dk"><div class="fill f-hot" data-w="18.89"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name" style="color:rgba(255,255,255,0.85);">2–3次</span><span class="hbar-pct" style="color:#FFD6E8;">39.17%</span></div>
      <div class="track dk"><div class="fill f-pk" data-w="39.17"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name" style="color:rgba(255,255,255,0.85);">1次</span><span class="hbar-pct" style="color:#FFD6E8;">31.80%</span></div>
      <div class="track dk"><div class="fill f-soft" data-w="31.80"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name" style="color:rgba(255,255,255,0.85);">0次（尚未查重）</span><span class="hbar-pct" style="color:rgba(255,255,255,0.5);">10.14%</span></div>
      <div class="track dk"><div class="fill f-lt" data-w="10.14"></div></div>
    </div>
  </div>

  <div class="div div-lt"></div>

  <!-- 图表8：价格对比图（带进度条） -->
  <p class="chart-title" style="color:rgba(255,255,255,0.55);">▌ 主流平台 2万字论文 单次双检费用对比（2026年实测）</p>
  <div class="price-wrap">
    <div class="pr-row">
      <div class="pr-top"><span class="pr-name">📚 知网 CNKI</span><span class="pr-amt">87.5<small> 元</small></span></div>
      <div class="pr-bar-track"><div class="pr-bar-fill" data-w="67"></div></div>
    </div>
    <div class="pr-row">
      <div class="pr-top"><span class="pr-name">🏫 学信网（万方）</span><span class="pr-amt">95<small> 元</small></span></div>
      <div class="pr-bar-track"><div class="pr-bar-fill" data-w="73"></div></div>
    </div>
    <div class="pr-row">
      <div class="pr-top"><span class="pr-name">📖 大雅</span><span class="pr-amt">100<small> 元</small></span></div>
      <div class="pr-bar-track"><div class="pr-bar-fill" data-w="77"></div></div>
    </div>
    <div class="pr-row">
      <div class="pr-top"><span class="pr-name">🔍 万方检测</span><span class="pr-amt">125<small> 元</small></span></div>
      <div class="pr-bar-track"><div class="pr-bar-fill" data-w="96"></div></div>
    </div>
    <div class="pr-row">
      <div class="pr-top"><span class="pr-name">📝 维普</span><span class="pr-amt">130<small> 元</small></span></div>
      <div class="pr-bar-track"><div class="pr-bar-fill" data-w="100"></div></div>
    </div>
  </div>

  <div style="background:rgba(255,255,255,0.08);border:1px solid rgba(255,255,255,0.15);border-radius:14px;padding:18px;margin-top:16px;">
    <p style="font-size:13px;color:rgba(255,255,255,0.88);line-height:1.9;"><strong style="color:#FFD6E8;">💡 费用真相：</strong>检测通常以"字符"计价，一个英文字母或标点也算一个字符。一篇2万字的论文，字符数可能达到<strong style="color:#FFD6E8;">2.5万字符</strong>以上，实际费用更高。若查重4次，仅知网一个平台累计支出已超<strong style="color:#FFD6E8;">350元</strong>；若同时使用多平台交叉验证，总支出轻松突破<strong style="color:#FFD6E8;">500元</strong>。</p>
    <p style="font-size:12.5px;color:rgba(255,255,255,0.65);font-style:italic;margin-top:12px;line-height:1.9;">"论文还没写完，检测费先花了几百。"<br>"查了5次知网，改了3轮，最后老师说格式还有问题。"<br>"我用了4个平台，每个结果都不一样，不知道相信哪个。"</p>
  </div>
</section>

<!-- ══ S6: 降重策略 · 雷达图 ══ -->
<section class="sec s-tl">
  <div class="badge" style="background:var(--tl)">06</div>
  <p class="eyebrow eyebrow-tl">降重行为分析</p>
  <h2 class="stitle">降重花样百出<br>但AI检测仍是另一道关</h2>
  <p class="body">在降重方面，94.47%的学生通过替换词汇、改写段落来降低重复率，82.95%使用线上降重工具辅助，67.28%删减重复、补充原创内容。然而，<strong>这些降重方式针对的是传统查重逻辑，在AI检测面前往往适得其反</strong>。大量的同义词替换和规则性句式变换，恰恰是AI写作的典型特征之一，这意味着降重和降AI率，很可能是一对相互矛盾的目标。</p>

  <!-- 图表9：SVG雷达图 -->
  <div class="radar-wrap">
    <p class="chart-title">▌ 学生主流降重方式占比（N=217）</p>
    <svg width="280" height="240" viewBox="0 0 280 240" style="overflow:visible">
      <!-- grid -->
      <g transform="translate(140,120)">
        <polygon points="0,-80 69,-40 69,40 0,80 -69,40 -69,-40" fill="none" stroke="#DDD0EA" stroke-width="1"/>
        <polygon points="0,-60 52,-30 52,30 0,60 -52,30 -52,-30" fill="none" stroke="#DDD0EA" stroke-width="1"/>
        <polygon points="0,-40 35,-20 35,20 0,40 -35,20 -35,-20" fill="none" stroke="#DDD0EA" stroke-width="1"/>
        <polygon points="0,-20 17,-10 17,10 0,20 -17,10 -17,-10" fill="none" stroke="#DDD0EA" stroke-width="1"/>
        <!-- axes -->
        <line x1="0" y1="0" x2="0" y2="-80" stroke="#C5A8D8" stroke-width="1"/>
        <line x1="0" y1="0" x2="69" y2="-40" stroke="#C5A8D8" stroke-width="1"/>
        <line x1="0" y1="0" x2="69" y2="40" stroke="#C5A8D8" stroke-width="1"/>
        <line x1="0" y1="0" x2="0" y2="80" stroke="#C5A8D8" stroke-width="1"/>
        <line x1="0" y1="0" x2="-69" y2="40" stroke="#C5A8D8" stroke-width="1"/>
        <line x1="0" y1="0" x2="-69" y2="-40" stroke="#C5A8D8" stroke-width="1"/>
        <!-- data: 94.47/82.95/67.28/58.99/58.99/58.99 → scale /100 * 80 -->
        <polygon
          points="0,-75.6 68.5,-33.2 53.8,21.8 0,47.2 -48.4,24.0 -66.8,-26.4"
          fill="rgba(201,79,124,0.25)" stroke="#C94F7C" stroke-width="2" stroke-linejoin="round"/>
        <!-- dots -->
        <circle cx="0" cy="-75.6" r="4" fill="#C94F7C"/>
        <circle cx="68.5" cy="-33.2" r="4" fill="#8B5C9E"/>
        <circle cx="53.8" cy="21.8" r="4" fill="#5BBCB8"/>
        <circle cx="0" cy="47.2" r="4" fill="#7BB8D4"/>
        <circle cx="-48.4" cy="24.0" r="4" fill="#F0894A"/>
        <circle cx="-66.8" cy="-26.4" r="4" fill="#E8729A"/>
        <!-- labels -->
        <text x="0" y="-88" text-anchor="middle" font-size="9.5" fill="#2D1A26" font-weight="600">替换词汇改写段落</text>
        <text x="76" y="-40" text-anchor="start" font-size="9.5" fill="#2D1A26" font-weight="600">线上降重工具</text>
        <text x="76" y="46" text-anchor="start" font-size="9.5" fill="#2D1A26" font-weight="600">删减补充原创</text>
        <text x="0" y="96" text-anchor="middle" font-size="9.5" fill="#2D1A26" font-weight="600">逐句调整语序</text>
        <text x="-76" y="46" text-anchor="end" font-size="9.5" fill="#2D1A26" font-weight="600">参考范文表述</text>
        <text x="-76" y="-40" text-anchor="end" font-size="9.5" fill="#2D1A26" font-weight="600">其他方式</text>
        <!-- scale labels -->
        <text x="3" y="-20" font-size="7" fill="#9B8AAA">25%</text>
        <text x="3" y="-40" font-size="7" fill="#9B8AAA">50%</text>
        <text x="3" y="-60" font-size="7" fill="#9B8AAA">75%</text>
      </g>
    </svg>
    <div class="radar-leg">
      <div class="radar-leg-item"><div class="radar-leg-dot" style="background:#C94F7C"></div>替换词汇 94.47%</div>
      <div class="radar-leg-item"><div class="radar-leg-dot" style="background:#8B5C9E"></div>线上工具 82.95%</div>
      <div class="radar-leg-item"><div class="radar-leg-dot" style="background:#5BBCB8"></div>删减补充 67.28%</div>
      <div class="radar-leg-item"><div class="radar-leg-dot" style="background:#7BB8D4"></div>调整语序 58.99%</div>
      <div class="radar-leg-item"><div class="radar-leg-dot" style="background:#F0894A"></div>参考范文 58.99%</div>
    </div>
  </div>

  <div class="qb" style="margin-top:4px;">
    ⚠ 一个残酷的现实是：传统降重（如大量替换词汇）反而可能提高AI检测率，因为AI改写的典型特征之一，正是大量的同义词替换和规则性句式变换。<strong>降重和降AI率，很可能是一对相互矛盾的目标</strong>——传统查重与AI检测之间，存在天然的技术张力。学生被迫在两套逻辑中反复横跳，精疲力竭。
  </div>

  <!-- 降重次数统计 -->
  <div class="anno">
    <p>📊 <strong>降重经济账：</strong>以一篇2万字论文为例，若需查重4次（约37%学生的实际情况），仅知网一个平台支出已达350元；若另购线上降重服务（均价约30–80元/次），总支出可能超过<strong>600元</strong>——这对许多尚未工作的大学生而言是不小的经济负担。</p>
  </div>
</section>

<svg class="wave" viewBox="0 0 480 24" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg"><path d="M0,0 C120,24 360,0 480,16 L480,24 L0,24Z" fill="var(--pkp)"/></svg>

<!-- ══ S7: 学生态度 · 环形+水平条 ══ -->
<section class="sec s-pk">
  <div class="badge">07</div>
  <p class="eyebrow">学生诉求与态度</p>
  <h2 class="stitle">支持规范<br>但坚决反对"一刀切"</h2>
  <p class="body">面对双检制度，学生的态度复杂而理性。超过六成学生基本支持双检制度，认为规范学术风气是必要的。但<strong>学生并非反对学术规范本身，而是反对"用一套不成熟的技术来做生死判决"</strong>的方式。"优化算法、减少误判"成为最强烈的呼声——这恰恰反映了当前AI检测技术最大的痛点：连技术本身都不够可靠，却要用它决定学生能否毕业。</p>

  <!-- 图表10：SVG环形图（态度分布） -->
  <div class="donut-row" style="margin-top:22px;">
    <svg width="130" height="130" viewBox="0 0 42 42">
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#EDD5E5" stroke-width="9"/>
      <!-- 非常支持 28% -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#C94F7C" stroke-width="9"
        stroke-dasharray="28 72" stroke-dashoffset="25"/>
      <!-- 基本支持 35% -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#8B5C9E" stroke-width="9"
        stroke-dasharray="35 65" stroke-dashoffset="-3"/>
      <!-- 中立 22% -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#5BBCB8" stroke-width="9"
        stroke-dasharray="22 78" stroke-dashoffset="-38"/>
      <!-- 不太支持/坚决反对 15% -->
      <circle cx="21" cy="21" r="15.915" fill="none" stroke="#F0894A" stroke-width="9"
        stroke-dasharray="15 85" stroke-dashoffset="-60"/>
      <text x="21" y="19.5" text-anchor="middle" font-size="4.5" font-weight="bold" fill="#C94F7C">63%</text>
      <text x="21" y="24" text-anchor="middle" font-size="3.5" fill="#6B6B6B">支持双检</text>
    </svg>
    <div class="dleg">
      <div class="drow"><div class="ddot" style="background:#C94F7C"></div><span class="dtxt">非常支持，规范学术风气</span><span class="dpct" style="color:#C94F7C">28%</span></div>
      <div class="drow"><div class="ddot" style="background:#8B5C9E"></div><span class="dtxt">基本支持，建议放宽标准</span><span class="dpct" style="color:#8B5C9E">35%</span></div>
      <div class="drow"><div class="ddot" style="background:#5BBCB8"></div><span class="dtxt">中立，利弊共存</span><span class="dpct" style="color:#5BBCB8">22%</span></div>
      <div class="drow"><div class="ddot" style="background:#F0894A"></div><span class="dtxt">不太支持/坚决反对</span><span class="dpct" style="color:#F0894A">15%</span></div>
    </div>
  </div>

  <!-- 图表11：诉求水平条形图 -->
  <div class="hbar-wrap" style="margin-top:8px;">
    <p class="chart-title">▌ 学生对双检规则调整的核心诉求排行（N=217）</p>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">优化AI检测算法，减少误判</span><span class="hbar-pct">76.50%</span></div>
      <div class="hbar-sub">最强烈呼声，指向当前AI检测技术最大痛点</div>
      <div class="track"><div class="fill f-hot" data-w="76.50"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">放宽论文重复率合格标准</span><span class="hbar-pct">70.51%</span></div>
      <div class="hbar-sub">认为当前查重红线在某些学科过于苛刻，应按学科差异化调整</div>
      <div class="track"><div class="fill f-pk" data-w="70.51"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">减少检测限制，降低收费</span><span class="hbar-pct">61.75%</span></div>
      <div class="hbar-sub">认为检测应由学校统一提供免费通道，而非全由学生自费</div>
      <div class="track"><div class="fill f-soft" data-w="61.75"></div></div>
    </div>
    <div class="hbar-item">
      <div class="hbar-meta"><span class="hbar-name">明确AI合理使用的边界</span><span class="hbar-pct">53.00%</span></div>
      <div class="hbar-sub">支持学校给出更清晰的"红绿灯"：什么能用，什么不能用</div>
      <div class="track"><div class="fill f-bl" data-w="53.00"></div></div>
    </div>
  </div>

  <p class="body" style="margin-top:14px;">值得关注的是，学生的态度中透露出一种<strong>理性与无奈并存</strong>的底色：他们并不反对学术诚信的本质要求，也能理解高校在AI时代面临的管理困境。但他们同时也清楚，<strong>一套标准不统一、技术不成熟、结果不稳定的检测体系，无法真正解决学术诚信的问题</strong>，只会制造更多焦虑和规避行为。</p>

  <div class="tag-row">
    <span class="tag t-pk">优化算法</span>
    <span class="tag t-pu">统一标准</span>
    <span class="tag t-pk">明确边界</span>
    <span class="tag t-tl">学科差异化</span>
    <span class="tag t-pu">降低费用</span>
    <span class="tag t-pk">学校提供免费通道</span>
    <span class="tag t-tl">透明化检测逻辑</span>
  </div>
</section>

<!-- CONCLUSION -->
<section class="conclusion">
  <span class="con-icon">💡</span>
  <h2 class="con-title">技术向善，<br>还是技术向"拷"？</h2>
  <p class="con-body">
    2026年，当AI写作工具已经深度嵌入大学生的学习和写作流程时，高校选择用"检测"来应对，而非"引导"。<br><br>
    有评论指出，如果为了防止学生使用AI，"AI检测"和过去一些学校的查重一样，变成无谓的折腾乃至经济负担，恐怕就滑向形式主义了。AI检测工具并不成熟，不同平台数据差异巨大，逻辑严谨的原创内容频频被标红。<strong style="color:#FFD6E8;">用一套不成熟的技术去评判一个学生能否毕业，这本身就是一个需要反思的问题。</strong><br><br>
    问题的核心或许不在于"用不用AI"，而在于如何界定"合理使用"与"学术不端"的边界。北京工商大学要求标注AI使用场景和工具名称的做法，或许提供了一种思路——与其把AI当作敌人严防死守，不如<strong style="color:#FFD6E8;">教会学生如何正确使用这个工具</strong>。AI工具使用应坚持"人工主导、AI辅助"的原则。技术本身无所谓善恶，关键在于使用技术的人，以及规范技术使用的制度。<br><br>
    当97%的学生都在用AI写论文时，我们需要思考的或许不是"怎么禁止"，而是"怎么引导"——让AI成为提升学术能力的工具，而非绕过学术训练的手段。这比任何检测算法都更重要。
  </p>
  <div>
    <span class="con-pill">人工主导</span>
    <span class="con-pill">AI辅助</span>
    <span class="con-pill">合理引导</span>
    <span class="con-pill">技术向善</span>
    <span class="con-pill">透明标准</span>
    <span class="con-pill">学术公平</span>
  </div>
</section>

<!-- FOOTER -->
<div class="footer">
  数据来源：《大学生毕业论文查重情况调查》有效样本 N=217<br>
  覆盖本科51.15% · 硕士32.72% · 博士16.13%<br>
  文科15.67% · 理科34.1% · 工科29.03% · 农学/医学21.2%<br>
  二次数据：中国青年报 · 人民日报 · 各高校教务处公开文件<br>
  ——<br>
  中国海洋大学文学与新闻传播学院 · 2026年春季学期<br>
  《数据新闻与可视化》课程 · 任课教师：王玺<br>
  第六小组：马尚 · 金福美 · 林漫玲 · 耿艺桐 · 吴悠
</div>

<script>
// 横向条形图动画
document.querySelectorAll('.fill[data-w], .pr-bar-fill[data-w]').forEach(el => {
  el.style.width = '0%';
  new IntersectionObserver(([e]) => {
    if(e.isIntersecting){ el.style.width = el.dataset.w + '%'; }
  }, {threshold:0.15}).observe(el);
});

// 堆叠条形图动画
document.querySelectorAll('.seg[data-w]').forEach(el => {
  el.style.width = '0%';
  new IntersectionObserver(([e]) => {
    if(e.isIntersecting){ el.style.width = el.dataset.w + '%'; }
  }, {threshold:0.15}).observe(el);
});

// 棒棒糖图：动态移动圆点
document.querySelectorAll('.lp-line-wrap').forEach(wrap => {
  const line = wrap.querySelector('.lp-line');
  const dot = wrap.querySelector('.lp-dot');
  if(!line || !dot) return;
  const w = parseFloat(line.dataset.w) || 0;
  new IntersectionObserver(([e]) => {
    if(e.isIntersecting){
      const pct = w / 100;
      line.style.width = pct * 100 + '%';
      dot.style.right = 'auto';
      dot.style.left = 'calc(' + (pct * 100) + '% - 7px)';
    }
  }, {threshold:0.15}).observe(wrap);
});
</script>
</body>
</html>
