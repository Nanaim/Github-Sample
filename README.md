# Github-Sample
public static void userLogin(HashMap<String,String> input) throws InterruptedException{
	//	UIDriver.clickElementDynamic("FETBOE","FET BOE");		
	//Reporter.reportAll("Pass", "Switch to BOE app", "BOE Home page", "Navigation to BOE Successful", "Navigation to BOE Failed");
		{             
            UIDriver.clickElement("Setup");   
            UIDriver.setValue("QuickSearch",input.get("specName"));
            UIDriver.clickElement("Searchicon");
            Thread.sleep(5000);
            UIDriver.clickElementDynamic("UserHyperlink",input.get("specName"));
            UIDriver.clickElement("UserLoginButton");
            Thread.sleep(5000);
