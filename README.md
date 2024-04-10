
# Rapport

Namn på appen har ändrats, internetåtkomst har lagts till, och JavaScript har aktiverats (enabled).
Har lagt in en internal och external web, där external visar HIS-hemsida. En funktion för att
visa HIS.se har skapats som kallas "showExternalWebPage()" där url har inkluderats i en WebView.
För att växla mellan internal och external har sedan denna funktion infogats i funktionen 
"onOptionsItemSelected(MenuItem item)". Se kodsnuttar nedan. Samma sak har gjorts för internal
men då med koppling till html-dokumentet "about.html".

Kodexempel för att visa external web, och sedan kalla på denna funktion i drop-down menyn:
```
    public void showExternalWebPage(){
        myWebView.loadUrl("https://his.se");
    }
    
    if (id == R.id.action_external_web) {
        showExternalWebPage();
        Log.d("==>","Will display external web page");
        return true;
    }
```

Skärmdumpar på internal och external WebView:

![](Screenshot_internal.png)
![](Screenshot_external.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
