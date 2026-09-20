<template>
  <div class="page campus-3d-page">
    <section class="campus-3d-hero">
      <div>
        <span class="section-kicker"><i></i> 津南校区互动探索</span>
        <h1>3D 校园地图</h1>
        <p>在浏览器中进入南开大学津南校区三维地图，探索道路、图书馆、公共自行车与校园环境。</p>
      </div>
      <a class="button primary" href="/campus-3d/index.html?quality=ultra" target="_blank" rel="noopener">全屏打开地图 <span>→</span></a>
    </section>

    <section class="campus-3d-frame" aria-label="南开大学津南校区 3D 互动地图">
      <iframe
        src="/campus-3d/index.html?quality=ultra"
        title="南开大学津南校区 3D 互动地图"
        allow="autoplay"
      ></iframe>
    </section>

    <aside class="safety-banner campus-3d-note">
      <span class="safety-symbol" aria-hidden="true">3D</span>
      <div>
        <strong>本页面用于校园探索演示</strong>
        <p>建筑开放时间、办事地点与应急信息请以学校官方通知及本网站对应指南为准。</p>
      </div>
    </aside>
  </div>
</template>

<style scoped>
.campus-3d-page { display: grid; gap: 1.25rem; }
.campus-3d-hero { display: flex; align-items: end; justify-content: space-between; gap: 2rem; padding: clamp(1.5rem, 4vw, 3rem); border-radius: 1.25rem; background: linear-gradient(135deg, #103f46, #1b6971); color: #fff; }
.campus-3d-hero h1 { margin: .45rem 0; font-size: clamp(2rem, 4vw, 3.5rem); }
.campus-3d-hero p { max-width: 42rem; margin: 0; color: rgba(255,255,255,.82); line-height: 1.7; }
.campus-3d-frame { overflow: hidden; min-height: 42rem; border: 1px solid rgba(20, 71, 73, .2); border-radius: 1.25rem; background: #102e32; box-shadow: 0 1rem 2rem rgba(8, 39, 42, .12); }
.campus-3d-frame iframe { display: block; width: 100%; height: 70vh; min-height: 42rem; border: 0; }
.campus-3d-note { margin: 0; }
@media (max-width: 700px) { .campus-3d-hero { align-items: flex-start; flex-direction: column; } .campus-3d-frame, .campus-3d-frame iframe { min-height: 34rem; } }
</style>
