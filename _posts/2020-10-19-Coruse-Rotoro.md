---
layout: post
title: Лабораторная №1, курс Kubernetes для самых маленьких
---
<script src="/jquery.min.js"></script>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.4/css/bootstrap.min.css" integrity="2hfp1SzUoho7/TsGGGDaFdsuuDL0LX2hnUp6VkX3CUQ2K4K+xjboZdsXyp4oUHZj" crossorigin="anonymous">
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.4/js/bootstrap.min.js" integrity="VjEeINv9OSwtWFLAtmc4JCtEJXXBub00gtSnszmspDLCtC0I4z4nqz7rEFbIZLLU" crossorigin="anonymous"></script>

<div>
    <div class="attachment-data"></div>
    
      <div id="rt_scenario" name="kubernetes-for-beginners-ru"></div>
    
</div>


<script>
    var scenario_div_name = '#rt_scenario';
    
    var startLab = function(){
        $('#start-lab-button').remove();
        
        var scenario_name = $(scenario_div_name).attr('name')
        var lab_name = $('#rt_scenario').attr("lab")
        var data_katacoda_command = "";
        if(lab_name){
            data_katacoda_command="export SCENARIO_NAME=" + lab_name + ";";
        }
        
        var div_source_code = '<div id="katacoda-scenario-1" data-katacoda-command="' + data_katacoda_command + '" data-katacoda-hideintro="false" data-katacoda-id="rotoro-cloud/' + scenario_name + '" data-katacoda-externalcss="https://raw.githubusercontent.com/rotoro-cloud/rotoro-cloud.github.io/master/labEnv.css" data-katacoda-color="004d7f" style="height: 90vh;">';
        $(scenario_div_name).append(div_source_code);    
        var embed_script = document.createElement('script');
        embed_script.setAttribute('src','https://katacoda.com/embed.js?cache=rt');
        
        if($(scenario_div_name + ' script').length == 0){
            $(scenario_div_name).append(embed_script);
        }
    
      
    }
    
    var div_button_source_code = '<div style="text-align: center;"><img src="https://raw.githubusercontent.com/rotoro-cloud/rotoro-cloud.github.io/master/images/KFB/lab01.jpg" onclick="startLab()" style="margin-top: 20px;"><div id="start-lab-button" style="margin-top: 20px;"><a class="btn btn-md btn-primary" onclick="startLab()" >Запуск упражнения</a><br><br><a href="https://rotoro.cloud/troubleshooting-labs" target="_blank">Если возникли проблемы, смотри здесь</a></div></div>';
    
    $(scenario_div_name).append(div_button_source_code);  

</script>


<script>
  
  $(document).ready(function() { 
    if($('#rt_feedback_form')){
    var course=$('#rt_feedback_form').attr('course')
    var section=$('#rt_feedback_form').attr('section')
    
    var entries = ""
    if(typeof userid !== 'undefined'){
        var entries="&entry.1103390199=" + section + "-" + userid
    }
    
  }
    
  });
  
</script>
