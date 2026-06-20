<template>
  <div class="page-shell">
    <header class="hero">
      <div class="hero-copy">
        <p class="eyebrow">Conservation Desk</p>
        <h1>古籍虫蛀修复批次板</h1>
        <p class="lead">
          给纸本文献修复工作室使用的轻量前端，用来查看虫蛀页批次、控湿策略和修复优先级。
        </p>
      </div>
      <div class="hero-stat">
        <span>待处理批次</span>
        <strong>12 册</strong>
        <p>高湿季节前完成封边与补纸。</p>
      </div>
    </header>

    <main class="layout">
      <section class="panel wide">
        <div class="panel-head">
          <h2>批次概览</h2>
          <span class="chip">本周计划</span>
        </div>
        <div class="batch-grid">
          <article class="batch-card active">
            <small>批次 A-03</small>
            <h3>明抄本县志残卷</h3>
            <p>页码 17-29，虫道集中在装订线外沿。</p>
          </article>
          <article class="batch-card">
            <small>批次 B-11</small>
            <h3>碑帖拓片册页</h3>
            <p>需先降湿 48 小时，再进入纤维加固。</p>
          </article>
          <article class="batch-card">
            <small>批次 C-02</small>
            <h3>戏曲抄本散页</h3>
            <p>边角缺损明显，建议先做透明托裱。</p>
          </article>
        </div>
      </section>

      <section class="panel">
        <div class="panel-head">
          <h2>环境参数</h2>
          <span class="chip soft">修复室 2</span>
        </div>
        <div class="gauge-list">
          <div class="gauge-card">
            <span>相对湿度</span>
            <strong>52%</strong>
            <p>控制线 50% - 55%</p>
          </div>
          <div class="gauge-card">
            <span>纸浆补配</span>
            <strong>2 批</strong>
            <p>桑皮纤维待过滤</p>
          </div>
          <div class="gauge-card">
            <span>紫外检查</span>
            <strong>4 页</strong>
            <p>夜间统一复核霉斑残留</p>
          </div>
        </div>
      </section>

      <section class="panel">
        <div class="panel-head">
          <h2>修复工序</h2>
          <span class="chip">今日流程</span>
        </div>
        <ol class="step-list">
          <li>拍照建档并标注虫蛀起止页。</li>
          <li>低压吸附除尘，保留边角碎纤维。</li>
          <li>喷雾回软后局部补纸，不做整页过度清洗。</li>
          <li>平整定型 8 小时后转入无酸盒暂存。</li>
        </ol>
      </section>

      <section class="panel wide">
        <div class="panel-head">
          <h2>任务清单</h2>
          <span class="chip">按风险排序</span>
        </div>
        <div class="task-table">
          <div class="task-row task-head">
            <span>对象</span>
            <span>阶段</span>
            <span>风险</span>
            <span>说明</span>
          </div>
          <div class="task-row">
            <span>明抄本县志残卷</span>
            <span>补纸前</span>
            <span class="tag high">高</span>
            <span>虫道贯穿标题栏，需先固色</span>
          </div>
          <div class="task-row">
            <span>碑帖拓片册页</span>
            <span>控湿中</span>
            <span class="tag medium">中</span>
            <span>边缘卷曲，可延后压平</span>
          </div>
          <div class="task-row">
            <span>戏曲抄本散页</span>
            <span>归档前</span>
            <span class="tag low">低</span>
            <span>等待封套尺寸确认</span>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>
