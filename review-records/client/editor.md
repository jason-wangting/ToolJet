# main editor
1. use `zustand` to store global state, there are two main store: `AppDataStore` and `EditorStore`. We only need focusing on EditorState
2. `EditorHeader` component to show the header of application
3. `LeftSidebar` to show the left sidebar and left sidebar popover.
4. `QueryPanel` shows in the below
5. `RightSidebar` shows in the right
6. get `appDefinition` -> `computeComponentState` -> `defaultComponentStateComputed = true` -> render `Container` Component

# Used Library
1. `react-hotkeys-hook` A React hook for using keyboard shortcuts in components in a declarative way.
    ```
        import { useHotkeys } from 'react-hotkeys-hook'
        export const ExampleComponent = () => {
        const [count, setCount] = useState(0)
        useHotkeys('ctrl+k', () => setCount(count + 1), [count])

        return (
            <p>
            Pressed {count} times.
            </p>
        )
        }
    ```