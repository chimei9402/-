<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <meta charset="UTF-8">
  <title>慢性病族群身心社會功能整合評估表</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: "Noto Sans TC", Arial, sans-serif;
      background: #f6f7f8;
      padding: 20px;
    }
    .container {
      max-width: 800px;
      background: #fff;
      padding: 25px;
      border-radius: 8px;
      margin: auto;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    h1 {
      text-align: center;
      margin-bottom: 10px;
    }
    .desc {
      text-align: center;
      color: #555;
      margin-bottom: 30px;
    }
    .group {
      margin-bottom: 20px;
    }
    label {
      font-weight: bold;
      display: block;
      margin-bottom: 8px;
    }
    .options label {
      font-weight: normal;
      display: block;
      margin: 4px 0;
    }
    input[type="text"] {
      width: 100%;
      padding: 8px;
      box-sizing: border-box;
    }
    button {
      width: 100%;
      padding: 12px;
      background: #2c7be5;
      color: white;
      border: none;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
    }
    button:hover {
      background: #1a5fc1;
    }
  </style>
</head>
<body>

<div class="container">
  <h1>慢性病族群身心社會功能整合評估表</h1>
  <p class="desc">請根據您「過去一個月」的真實感受，勾選最符合的選項。</p>

  <form onsubmit="submitForm(event)">
    <div class="group">
      <label>個案姓名</label>
      <input type="text" name="name">
    </div>

    <div class="group">
      <label>性別</label>
      <div class="options">
        <label><input type="radio" name="gender"> 男</label>
        <label><input type="radio" name="gender"> 女</label>
        <label><input type="radio" name="gender"> 其他</label>
      </div>
    </div>

    <div class="group">
      <label>年齡</label>
      <div class="options">
        <label><input type="radio" name="age"> 20~30歲</label>
        <label><input type="radio" name="age"> 31~40歲</label>
        <label><input type="radio" name="age"> 41~50歲</label>
        <label><input type="radio" name="age"> 51~60歲</label>
        <label><input type="radio" name="age"> 61~70歲</label>
        <label><input type="radio" name="age"> 71~80歲</label>
        <label><input type="radio" name="age"> 80歲以上</label>
        <label><input type="radio" name="age"> 無意願透露</label>
      </div>
    </div>

    <div class="group">
      <label>Q1 身體感受</label>
      <div class="options">
        <label><input type="radio" name="q1"> 非常好</label>
        <label><input type="radio" name="q1"> 還不錯</label>
        <label><input type="radio" name="q1"> 普通</label>
        <label><input type="radio" name="q1"> 不太好</label>
        <label><input type="radio" name="q1"> 很不好</label>
      </div>
    </div>

    <div class="group">
      <label>Q2 經濟負擔</label>
      <div class="options">
        <label><input type="radio" name="q2"> 完全沒有</label>
        <label><input type="radio" name="q2"> 有一點</label>
        <label><input type="radio" name="q2"> 普通</label>
        <label><input type="radio" name="q2"> 很有壓力</label>
        <label><input type="radio" name="q2"> 壓力很大</label>
      </div>
    </div>

    <div class="group">
      <label>Q3 資源支應</label>
      <div class="options">
        <label><input type="radio" name="q3"> 足夠</label>
        <label><input type="radio" name="q3"> 大致夠</label>
        <label><input type="radio" name="q3"> 普通</label>
        <label><input type="radio" name="q3"> 有點不夠</label>
        <label><input type="radio" name="q3"> 很不夠</label>
      </div>
    </div>

    <div class="group">
      <label>Q4 心理情緒</label>
      <div class="options">
        <label><input type="radio" name="q4"> 完全沒有</label>
        <label><input type="radio" name="q4"> 有一點</label>
        <label><input type="radio" name="q4"> 普通</label>
        <label><input type="radio" name="q4"> 有影響</label>
        <label><input type="radio" name="q4"> 影響很大</label>
      </div>
    </div>

    <div class="group">
      <label>Q5 飲食執行</label>
      <div class="options">
        <label><input type="radio" name="q5"> 完全不會</label>
        <label><input type="radio" name="q5"> 有一點</label>
        <label><input type="radio" name="q5"> 普通</label>
        <label><input type="radio" name="q5"> 有困難</label>
        <label><input type="radio" name="q5"> 非常困難</label>
      </div>
    </div>

    <div class="group">
      <label>Q6 活動體能</label>
      <div class="options">
        <label><input type="radio" name="q6"> 完全沒有</label>
        <label><input type="radio" name="q6"> 有一點</label>
        <label><input type="radio" name="q6"> 普通</label>
        <label><input type="radio" name="q6"> 有影響</label>
        <label><input type="radio" name="q6"> 影響很大</label>
      </div>
    </div>

    <div class="group">
      <label>Q7 社交支持</label>
      <div class="options">
        <label><input type="radio" name="q7"> 有穩定、固定的人</label>
        <label><input type="radio" name="q7"> 有，但不一定或不固定</label>
        <label><input type="radio" name="q7"> 幾乎沒有</label>
      </div>
    </div>

    <div class="group">
      <label>Q8 決策支持</label>
      <div class="options">
        <label><input type="radio" name="q8"> 有穩定、固定的人</label>
        <label><input type="radio" name="q8"> 有，但不一定或不固定</label>
        <label><input type="radio" name="q8"> 幾乎沒有</label>
      </div>
    </div>

    <button type="submit">送出評估表</button>
  </form>
</div>

<script>
  function submitForm(e) {
    e.preventDefault();
    alert("已成功送出，謝謝您的填寫！");
  }
</script>

</body>
</html>
