# Origin data

The original data has the same format with RQ1

```json
{
    "944e308a52e985e2498287a82f71dd4e03fc1724":     // The commit hash
    {
        "ResponseEntityProxy":  // name of changed class
        [
            {
                "method": "writeTo",    // name of changed method
                "type": "add",  // type of change
                "ast": 14,  // amount of AST affected
                "importance": 0.0,  // the importance of the changed location,
                "complex_middle":   // complexity metrics
                [
                    110.68527648135249,     // not used
                    106.2,  // Halstead Volume
                    2.0,    // CC
                    9.0,    // LoC
                    0.0     // Percentage of comment
                ], 
                "dataflow":     // Impact range
                [
                    {
                        "forward": 3,   // forward trace
                        "backward": 3,  // backward trace
                        "total": 14,    // total nodes
                        "changed_node": 8   // total changed node
                    }
                ]
            }
        ]
    }
}
```
