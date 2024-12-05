<h1 id="contact"></h1>

<h2 style="margin: 30px 0px 10px;">Contact</h2>

<p><strong>Address:</strong> <a href="https://www.google.fr/maps/place/%E4%B8%8A%E6%B5%B7%E7%A7%91%E6%8A%80%E5%A4%A7%E5%AD%A6/@31.1763741,121.5898769,17z/data=!3m1!4b1!4m6!3m5!1s0x35b27828f381499b:0x5ae88f32ad8196b1!8m2!3d31.1763741!4d121.5924518!16s%2Fm%2F0qftcsg?entry=ttu" rel="noopener noreferrer" target="_blank">393 Middle Huaxia Road, Pudong, Shanghai, China</a>
<br />
<strong>Office Location:</strong> 305-D, School of Biomedical Engineering, ShanghaiTech University
<br />
<strong>Email:</strong> <email>douyl2023[at]shanghaitech.edu.cn</email>
<br />

<!-- global map 世界地图 -->
<!-- <script type="text/javascript" src="//rf.revolvermaps.com/0/0/6.js?i=5nrmyu6wxer&amp;m=8&amp;c=baff00&amp;cr1=ffc000&amp;f=arial&amp;l=1" async="async"></script> -->
<script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=cLum3i28f8lNkgXT8de4QA7iBb9gX70DftFpLAinJ3U"></script>


<!-- footer -->
<hr style="border: 0.5px solid #ddd; margin-top: 30px;">
<div style="display: flex; justify-content: space-between; align-items: center; padding: 10px 0; font-size: 14px;">
    <div id="last-update">
        © Yulong Dou <br>
        <span id="update-time">- Last Update: </span>
    </div>
    <div style="display: flex; gap: 10px;">
        <img src="./assets/img/ShanghaiTech_Logo.png" alt="Logo 1" style="height: 50px;">
        <img src="./assets/img/impact_logo.jpg" alt="Logo 2" style="height: 50px;">
    </div>
</div>


<script>
    document.addEventListener('DOMContentLoaded', function () {
        const updateElement = document.getElementById('update-time');
        const lastUpdate = new Date(document.lastModified);
        
        // Convert time to UTC+8 (East Asia time zone)
        const utc8Offset = 8 * 60; // 8 hours in minutes
        const localTime = new Date(lastUpdate.getTime() + (utc8Offset * 60 * 1000));
        
        const year = localTime.getUTCFullYear();
        const month = String(localTime.getUTCMonth() + 1).padStart(2, '0');
        const day = String(localTime.getUTCDate()).padStart(2, '0');
        const hours = String(localTime.getUTCHours()).padStart(2, '0');
        const minutes = String(localTime.getUTCMinutes()).padStart(2, '0');
        
        const formattedDate = `${year}-${month}-${day} ${hours}:${minutes} UTC+8`;
        updateElement.textContent += formattedDate;
    });
</script>
