---
pageClass: dashboard
title: Dashboard
sidebar: false
copyright:
  noCopy: true
  noSelect: true
Optimization:
  spam: 0
  revision:  0
  overhead: 5.8
Perfomance:
  date: 2022-01-07
  loadTime: 1.7
  Region: London (UK)
pageSpeed:
  grade: B
  result: 83%
  previous: B (83%)
ySlow:
  grade: B
  result: 81%
  previous: B (81%)
Backup:
  latest: 20 Dicembre 2021
  next: 2022-01-20
  details: [ "OceanWP v3.1.1", "Versione WP: 5.8.2", "Plugins: 28", "Numero di Posts: 0", "Commenti Approvati: 0" ]
  total:  397.35
  files: 274.02
  db: 123.323
Security:
  latest: 2022-01-07T11:37:00
  Checks: [ "Malware: Clean", "Vulnerabilities: Clean", "WebTrust: Clean" ]
Availability:
  up: 100
  downtimes: 0
  timedown: 0 Ore 0 Min
  month: "Gennaio"
---

<main
    data-color-mode="auto"
    data-light-theme="light"
    data-dark-theme="dark_dimmed"
    class="d-flex flex-justify-between flex-column flex-sm-row  flex-md-items-start">
<section
class="color-bg-subtle my-2 p-md-4 p-sm-2 border rounded col-sm-12 mx-1 col-md-8 flex-1">
<PerfomanceHeader />
<div class="d-flex flex-wrap flex-justify-around flex-sm-items-center">
<pageSpeed /> <ySlow />
</div>

<ChartBox>

```chart
{
"type": "line",
"width": "400",
"height": "400",
"data": {
"labels": ["1", "2", "3", "4", "5", "6", "7",
            "8", "9", "10", "11", "12", "13",
            "14", "15", "16", "17", "18", "19",
            "20", "21", "22", "23c", "24", "25",
            "26",  "27", "28", "29", "30", "31"
            ],
"datasets": [
{
"label": "Tempo di Caricamento (s)",
"data": [ 4, 6, 4, 7, 5, 5, 7,
          8, 4

          ],
"backgroundColor": "rgba(186, 218, 85, 0.4)",
"borderColor": "#bada55",
"borderWidth": 1
},
{
"label": "Dimensione Pagina (MB)",
"data": [ 3.48, 3.48, 3.49, 3.48, 3.48, 3.50, 3.48,
          3.49, 3.49


        ],
"backgroundColor": "rgba(117,85,218, 0.4)",
"borderColor": "#7555da",
"borderWidth": 1
}
]
},
"options": {
"scales": {
"yAxes": [{
"type": "linear",
"display": true,
"ticks": {
  "beginAtZero": false,
  "max": 20,
  "min": 0
}
}]
}
}
}
```
</ChartBox>

<div class="border color-bg-subtle my-4" >
  <p class="f5 pl-6 pt-2">Video Test <span class="text-small Label Label--inline">2021-11-20</span> </p>
  <div class="d-flex flex-wrap flex-justify-around">
      <video width="320" height="240" controls autoplay>
          <source src="/browsertime-results/energ-tech.it/2021-11-20T132942+0000/pages/energ-tech_it/data/video/1.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
          <video  width="320" height="240" controls autoplay>
          <source src="/browsertime-results/energ-tech.it/2021-11-20T132942+0000/pages/energ-tech_it/data/video/1.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
          <video  width="320" height="240" controls autoplay>
          <source src="/browsertime-results/energ-tech.it/2021-11-20T132942+0000/pages/energ-tech_it/data/video/1.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
  </div>
</div>

<OptimizationWidget />

<div class="container d-flex flex-column flex-sm-row">
  <DowntimeWidget class="col-sm-12 col-md-6 mx-auto" />

  <AxiosWp id="installed_plugins"  class="col-sm-12 col-md-6 color-bg-default rounded mt-3 color-bg-subtle">

  </AxiosWp>
</div>

</section>


<section class="col-sm-12 col-md-3 mx-2">


<BackupCard />
<SecurityCard />

<ScanBot />

<HttpsStatus />

<UpdatesCard>

<ThemesTimeline />
<PluginsTimeline />



</UpdatesCard>

</section>


</main>

<style>





</style>
