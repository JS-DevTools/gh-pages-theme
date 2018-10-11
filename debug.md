---
---

<pre id="json">
  {{ site | jsonify | xml_escape }}
</pre>

<script>
  let pre = document.getElementById('json');
  let json = pre.innerText;
  let pojo = JSON.parse(json);

  pre.innerText = JSON.stringify(pojo, null, 2);
</script>
