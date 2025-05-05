# Summary for ToolSwitch.cs

[PYTHON]
class ToolSwitch:
    def __init__(self):
        self.tool_a = False
        self.tool_b = False

    def switch(self):
        if self.tool_a:
            self.tool_a = False
            self.tool_b = True
        else:
            self.tool_a = True
            self.tool_b = False
[/PYTHON]
