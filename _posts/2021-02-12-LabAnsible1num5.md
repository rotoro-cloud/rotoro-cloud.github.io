---
layout: post
title: Лабораторная №5 (Variables), курс Ansible для самых маленьких
---

<div id="rt_scenario" image="ansible1/lab5.png" questions="ansible_variables_lab"></div>


<script>
    var scenario_div_name = '#rt_scenario';
    var scenario_image = $(scenario_div_name).attr('image');
    var scenario_questions = $(scenario_div_name).attr('questions');
    var div_button_source_code = '<div style="text-align: center;"><img id="lab-img" src="https://raw.githubusercontent.com/rotoro-cloud/rotoro-cloud.github.io/master/images/' + scenario_image + '" onclick="startLab()" style="margin-top: 20px;"><div id="start-lab-button" style="margin-top: 20px;"><a class="btn btn-md btn-primary" onclick="startLab()" >Запуск упражнения</a><br><br><a href="https://rotoro-cloud.github.io/labs-ts/" target="_blank">Если возникли проблемы, смотри здесь</a></div></div>'; 
    
    var startLab = function() {
        $('#start-lab-button').remove();
        $('#lab-img').remove();
        var div_source_code = ' <iframe height="100%" width="100%" src="https://rotoro-cloud.github.io/ansible-quiz/index.html#!/?questions=' + scenario_questions + '" frameborder="0" style="overflow:hidden;overflow-x:hidden;overflow-y:hidden;height:100%;width:100%;position:absolute;top:0px;left:0px;right:0px;bottom:0px" height="100%" width="100%"></iframe>';
        $(scenario_div_name).append(div_source_code);
     }
     
     $(document).ready(function() {
        $(scenario_div_name).append(div_button_source_code);  
     });
</script>
