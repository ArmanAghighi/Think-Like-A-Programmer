Automible class :
```
    public class Automobile
    {
        private string _automobileModelName;
        private string _automobileComponyName;
        private int _automobileProductYear;

        public void SetAutomobileModel(string moedelName)
        {
            _automobileModelName = moedelName;
        }

        public string GetAutomobileModel()
        {
            return _automobileModelName;
        }

        public void SetCompanyName(string companyName)
        {
            _automobileComponyName = companyName;
        }

        public string GetCompanyname()
        {
            return _automobileComponyName;
        }

        public void SetProductYear(int productYear)
        {
            _automobileProductYear = productYear;
        }

        public int GetProductYear()
        {
            return _automobileProductYear;
        }
    }
```

Program Class
```
    public static class program
    {
        private static void Main()
        {
            Automobile automobile = new Automobile();
            
            automobile.SetCompanyName("Chevrolet");
            automobile.SetAutomobileModel("Corvet Z06");
            automobile.SetProductYear(2013);
        }
    }
```