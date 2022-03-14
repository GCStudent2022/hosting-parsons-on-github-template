# Greycourt Parson Puzzles
Rearrange the blocks provided to create valid Python code.
Don't forget to indent code inside if / elif / else statements.


## Positive or negative
Rearrange the code to determine whether the number is positive or negative
<div id="parson2-sortableTrash" class="sortable-code"></div> 
<div id="parson2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="parson2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="parson2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "if num &gt; 0:\n" +
    "    print(&quot;Positive number&quot;)\n" +
    "else:\n" +
    "    print(&quot;Negative number&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "parson2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "parson2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#parson2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#parson2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Zero, positive or negative
rearrange the code to determine whether the number is zero, positive or negative
<div id="parson3-sortableTrash" class="sortable-code"></div> 
<div id="parson3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="parson3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="parson3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "if num == 0:\n" +
    "	print(&quot;Zero&quot;)\n" +
    "elif num &gt; 0:\n" +
    "    print(&quot;Positive number&quot;)\n" +
    "else:\n" +
    "    print(&quot;Negative number&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "parson3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "parson3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#parson3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#parson3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
