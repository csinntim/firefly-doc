﻿# Exercise - Returning The Selected Value result

Your **ShowOrdersWithEmployeeSelection** view class should look like :

```csdiff
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Text;
using System.Windows.Forms;
using Firefly.Box;
using Firefly.Box.UI.Advanced;
using ENV;
using ENV.Data;

namespace Northwind.Exercises.SelectionList.Views
{
    partial class ShowOrdersWithEmployeeSelectionView : Shared.Theme.Controls.Form
    {
        ShowOrdersWithEmployeeSelection _controller;
        public ShowOrdersWithEmployeeSelectionView(ShowOrdersWithEmployeeSelection controller)
        {
            _controller = controller;
            InitializeComponent();
        }

+       private void txtCustomerID_Expand()
+       {
+           new SelectCustomers().Run(_controller.Orders.CustomerID);
+       }
    }
}
```
