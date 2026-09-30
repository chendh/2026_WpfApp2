# WPF視窗飲料訂購系統ver 1
2026/9/23

## 本週進度

### WPF佈局元件：Grid

- Grid.RowDefinitions, Grid.ColumnDefinitions
- Grid.RowSpan, Grid.ColumnSpan

### WPF佈局元件：StackPanel

- Stack.Orientation：Vertical(垂直排列), Horizontal(水平排列)

### C#選擇結構：if-else, switch case, 三元運算子

### TextBox.TextChanged事件

### 透過事件來取得呼叫的元件：

```csharp
var targetTextBox = sender as TextBox;
var targetStackPanel = targetTextBox.Parent as StackPanel;
var targetNameLabel = targetStackPanel.Children[0] as Label;
```

### 將字串轉換成整數
```csharp
int.TryParse()
Convert.ToInt32()
```

# WPF視窗飲料訂購系統ver 2
2026/9/30

## 功能更新
1. 使用Slider避免使用者入數值錯誤
2. 加上RadioButton和CheckBox來記錄購買方式以及選購飲料品項
3. 將Slider和Label以資料繫結(data binding)連動
4. 使用Dictionary資料結構來儲存飲料品項和訂單內容
5. 動態取得使用者選取的訂單品項
6. 加上售價折扣算法

## 本週進度
### 輸入控制項：
- RadioButton 與 CheckBox：理解單選（GroupName）與複選／三態（IsThreeState）邏輯。
- Slider：學習數值範圍（Minimum / Maximum）、刻度控制（TickPlacement / IsSnapToTickEnabled）與事件監聽。

### Data Binding（資料繫結）：
- 學習 Binding 4 大要素、流向模式（TwoWay / OneWay）與更新時機（UpdateSourceTrigger）。
- 實作 Element Binding：在 XAML 中無需 Code-Behind，將 Label 的 Content 綁定至 Slider 的 Value，並使用 StringFormat 進行數字格式化。
