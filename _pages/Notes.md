---
layout: archive
title: "Project 1"
permalink: /Notes/
author_profile: true
---

{% include base_path %}




1.1 Solo Author

Refining time-space traffic diagrams: A simple multiple linear regression model, IEEE Transactions on Intelligent Transportation Systems, 2024
Portraying ride-hailing mobility using multi-day trip order data: A case study of Beijing, China, Transportation Research Part A, 2021 (2022 Key innovation in Transportation Sector, Ministry of Transport, China)
Spatial-temporal fractal of urban agglomeration travel demand, Physica A, 2020
Cooperative driving and a lane change-free road transportation system,  Chapter of IET Book  Traffic Information and Control, 2020
Research based on high-fidelity NGSIM vehicle trajectory datasets: A review. DOI: 10.13140/RG.2.2.11429.60643, 2017
Transforming Policy-Car Swerving for Mitigating Stop-and-Go Traffic Waves: A Practice-Oriented Jam-Absorption Driving Strategy, arXiv, 2026


  <style>

        /* 时间线容器 */
        .timeline-container {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        /* 时间线竖线 */
        .timeline-container::after {
            content: '';
            position: absolute;
            width: 2px;
            background-color: #3498db;
            top: 0;
            bottom: 0;
            left: 20px;
        }

        /* 单个时间线项目 */
        .timeline-item {
            position: relative;
            margin-bottom: 40px;
            padding-left: 60px;
        }

        /* 时间节点圆点 */
        .timeline-node {
            position: absolute;
            left: 10px;
            top: 5px;
            width: 20px;
            height: 20px;
            background: #fff;
            border: 3px solid #3498db;
            border-radius: 50%;
            z-index: 1;
        }

        /* 内容区域 */
        .content {
            position: relative;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        /* 时间标题 */
        .content h3 {
            color: #3498db;
            margin-bottom: 8px;
        }

        /* 时间日期 */
        .time {
            display: block;
            color: #666;
            font-size: 0.9em;
            margin-bottom: 10px;
        }

        /* 响应式设计 */
        @media (max-width: 600px) {
            .timeline-container::after {
                left: 10px;
            }
            
            .timeline-item {
                padding-left: 40px;
            }
            
            .timeline-node {
                left: 0;
            }
        }
    </style>
   <details><summary>点击展开 </summary>
  <div class="timeline-container">
        <!-- 2022 秋 -->
    <div class="timeline-item">
      <div class="timeline-node"></div>
        <div class="content">
                <h3>你好, EECS</h3>
                <span class="time">2022 秋</span>
                <p>入燕园，初窥计算机语言与 Github</p>
        </div>
    </div>
    </div>
</details>



## 111

{% assign paths = "nameofthemd.md" | split: "," %}

{% for post in site.Notes reversed %}
  {% for path in paths %}
    {% if post.path contains path %}
      {% include archive-single.html %}
      {% break %}
    {% endif %}
  {% endfor %}
{% endfor %}
