---
layout: post
title: Ок, rotoro!
---
<script src="jquery-3.5.1.min.js"></script>


##### Переозвучка

<script src="https://fast.wistia.com/embed/medias/kkvk5mb740.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_kkvk5mb740 videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/kkvk5mb740/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>


##### С новой презентахой


<script src="https://fast.wistia.com/embed/medias/wp34o887ov.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_wp34o887ov videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/wp34o887ov/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

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
        
        var div_source_code = '<div id="katacoda-scenario-1" data-katacoda-command="' + data_katacoda_command + '" data-katacoda-hideintro="false" data-katacoda-id="rotoro-cloud/' + scenario_name + '" data-katacoda-externalcss="https://res.cloudinary.com/cloudusthad/raw/upload/v1571161480/custom.css" data-katacoda-color="004d7f" style="height: 90vh;">';
        $(scenario_div_name).append(div_source_code);    
        var embed_script = document.createElement('script');
        embed_script.setAttribute('src','https://katacoda.com/embed.js?cache=rt');
        
        if($(scenario_div_name + ' script').length == 0){
            $(scenario_div_name).append(embed_script);
        }
    
        
        
        $.post( window.location.pathname + "/complete", function() {
          console.log("lecture completed")
        })
          .done(function() {
            console.log("lecture done")
          })
          .fail(function() {
            console.log("lecture complete failed")
          })
          .always(function() {
            console.log("lecture complete finished")
          });
        
        
    }
    
    var div_button_source_code = '<div id="start-lab-button" style="text-align: center; margin-top: 200px;"><a class="btn btn-md btn-primary" onclick="startLab()" >Запуск упражнения</a><br><br><a href="https://support.rotoro.cloud/troubleshooting-labs" target="_blank">Если возникли проблемы, смотри здесь</a></div>';
    
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
