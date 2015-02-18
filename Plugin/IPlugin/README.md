# IPlugin
```c#
public interface IPlugin : IEquatable<IPlugin>
{
	string Author { get; }
	string Description { get; }
	Window DisplayWindow { get; }
	string Name { get; }
	Version Version { get; }

	void OnDisabled();
	void OnEnabled();
	void OnInitialize();
	void OnPulse();
	void OnShutdown();
}
```