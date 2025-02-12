function doGet() {
  return HtmlService.createHtmlOutputFromFile('Index')
    .setTitle('Organoleptic Test');
}

function saveResponse(data) {
  var sheet = SpreadsheetApp.getActiveSpreadsheet().getSheetByName("Responses");
  if (!sheet) {
    sheet = SpreadsheetApp.getActiveSpreadsheet().insertSheet("Responses");
    sheet.appendRow(["Branch", "Size", "Gills", "Texture", "Smell", "Eyes", "Belly", "Status"]);
  }
  sheet.appendRow([data.branch, data.size, data.gills, data.texture, data.smell, data.eyes, data.belly, data.status]);
}
