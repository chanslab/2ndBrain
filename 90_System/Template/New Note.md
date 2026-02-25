<%*
let date = tp.date.now("YYYY-MM-DD");
let title = await tp.system.prompt("파일 제목을 입력하세요");
if (title == null) { title = "Untitled"; }
await tp.file.rename(`${date}_${title}`);
%>