---
layout: post
title: Лабораторная №6 (Conditionals), курс Ansible для самых маленьких
---


<script src="/jquery.min.js"></script>

<div style="margin:0px;padding:0px;overflow:hidden" id="rt_scenario">

<script>
    var scenario_div_name = '#rt_scenario';
    var div_button_source_code = '<div id="start-lab-button" style="text-align: center; margin-top: 10px;"><a class="btn btn-md btn-primary" onclick="startLab()" ><img src="https://raw.githubusercontent.com/rotoro-cloud/rotoro-cloud.github.io/master/images/ansible1/lab6.png">Запуск упражнения</a><br><br><a href="https://rotoro.cloud/troubleshooting-labs" target="_blank">Если возникли проблемы, смотри здесь</a></div>';  
    
    var startLab = function() {
        $('#start-lab-button').remove();
        var div_source_code = ' <iframe height="100%" width="100%" src="https://rotoro-cloud.github.io/ansible-quiz/index.html#!/?questions=ansible_conditionals_lab" frameborder="0" style="overflow:hidden;overflow-x:hidden;overflow-y:hidden;height:100%;width:100%;position:absolute;top:0px;left:0px;right:0px;bottom:0px" height="100%" width="100%"></iframe>';
        $(scenario_div_name).append(div_source_code);
     }
     
     $(document).ready(function() {
        $(scenario_div_name).append(div_button_source_code);  
     });
</script>



</div>


