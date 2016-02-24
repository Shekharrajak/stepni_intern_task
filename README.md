##### using [google app engine](https://developers.google.com/apps-script/overview)

      function doGet(e) {
          var url = 'https://docs.google.com/document/d/1W0swizgXUIsdmZmy-U3sdQs4ZX3f2Sr6marlibQwIRQ/edit?usp=sharing';
          var doc = DocumentApp.openByUrl(url);
          
          doc.getBody().appendParagraph(' rollnum | '+e.parameter.email+' & | '+e.parameter.mobile);
          window.location="http://shekharrajak.github.io/stepni_intern_task";
          redirect("http://shekharrajak.github.io/stepni_intern_task")
          return true;
       }
